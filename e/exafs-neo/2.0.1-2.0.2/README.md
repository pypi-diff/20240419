# Comparing `tmp/exafs_neo-2.0.1.tar.gz` & `tmp/exafs_neo-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exafs_neo-2.0.1.tar", last modified: Thu Mar 14 06:25:19 2024, max compression
+gzip compressed data, was "exafs_neo-2.0.2.tar", last modified: Fri Apr 19 04:41:30 2024, max compression
```

## Comparing `exafs_neo-2.0.1.tar` & `exafs_neo-2.0.2.tar`

### file list

```diff
@@ -1,45 +1,66 @@
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-03-14 06:25:19.082481 exafs_neo-2.0.1/
--rw-r--r--   0 andy       (501) staff       (20)    35198 2024-03-14 06:25:03.000000 exafs_neo-2.0.1/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)     5005 2024-03-14 06:25:19.082622 exafs_neo-2.0.1/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)     4601 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/README.md
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-03-14 06:25:19.080475 exafs_neo-2.0.1/exafs_neo/
--rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)      152 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/_version.py
--rw-r--r--   0 andy       (501) staff       (20)     3364 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/exafs.py
--rw-r--r--   0 andy       (501) staff       (20)     4906 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/exafs_fileobj.py
--rw-r--r--   0 andy       (501) staff       (20)     5854 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/exafs_pop.py
--rw-r--r--   0 andy       (501) staff       (20)      982 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/helper.py
--rw-r--r--   0 andy       (501) staff       (20)      905 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/import_lib.py
--rw-r--r--   0 andy       (501) staff       (20)     3453 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/individual.py
--rw-r--r--   0 andy       (501) staff       (20)     5896 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/ini_parser.py
--rwxr-xr-x   0 andy       (501) staff       (20)     1226 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/input_arg.py
--rw-r--r--   0 andy       (501) staff       (20)     7140 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/neoCrossOver.py
--rw-r--r--   0 andy       (501) staff       (20)     3351 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/neoFilePars.py
--rw-r--r--   0 andy       (501) staff       (20)     8856 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/neoMutator.py
--rw-r--r--   0 andy       (501) staff       (20)    13671 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/neoPars.py
--rw-r--r--   0 andy       (501) staff       (20)     2610 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/neoResult.py
--rw-r--r--   0 andy       (501) staff       (20)     3494 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/neoSelector.py
--rwxr-xr-x   0 andy       (501) staff       (20)     5758 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/parser.py
--rw-r--r--   0 andy       (501) staff       (20)     3158 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/pathObj.py
--rw-r--r--   0 andy       (501) staff       (20)     5115 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/pathrange.py
--rw-r--r--   0 andy       (501) staff       (20)     1290 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/pathrange_file.py
--rw-r--r--   0 andy       (501) staff       (20)    16809 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/exafs_neo/utils.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-03-14 06:25:19.081405 exafs_neo-2.0.1/exafs_neo.egg-info/
--rw-r--r--   0 andy       (501) staff       (20)     5005 2024-03-14 06:25:19.000000 exafs_neo-2.0.1/exafs_neo.egg-info/PKG-INFO
--rw-r--r--   0 andy       (501) staff       (20)      955 2024-03-14 06:25:19.000000 exafs_neo-2.0.1/exafs_neo.egg-info/SOURCES.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-03-14 06:25:19.000000 exafs_neo-2.0.1/exafs_neo.egg-info/dependency_links.txt
--rw-r--r--   0 andy       (501) staff       (20)       55 2024-03-14 06:25:19.000000 exafs_neo-2.0.1/exafs_neo.egg-info/entry_points.txt
--rw-r--r--   0 andy       (501) staff       (20)        1 2024-03-14 06:25:19.000000 exafs_neo-2.0.1/exafs_neo.egg-info/not-zip-safe
--rw-r--r--   0 andy       (501) staff       (20)       40 2024-03-14 06:25:19.000000 exafs_neo-2.0.1/exafs_neo.egg-info/requires.txt
--rw-r--r--   0 andy       (501) staff       (20)       10 2024-03-14 06:25:19.000000 exafs_neo-2.0.1/exafs_neo.egg-info/top_level.txt
--rw-r--r--   0 andy       (501) staff       (20)       79 2024-03-14 06:25:19.083166 exafs_neo-2.0.1/setup.cfg
--rw-r--r--   0 andy       (501) staff       (20)     1189 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/setup.py
-drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-03-14 06:25:19.082378 exafs_neo-2.0.1/tests/
--rw-r--r--   0 andy       (501) staff       (20)     4411 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/tests/test_EXAFS_analysis.py
--rw-r--r--   0 andy       (501) staff       (20)     3796 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/tests/test_exafs_pars.py
--rw-r--r--   0 andy       (501) staff       (20)     3062 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/tests/test_exafs_pathObj.py
--rw-r--r--   0 andy       (501) staff       (20)     1573 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/tests/test_exafs_pathrange.py
--rw-r--r--   0 andy       (501) staff       (20)      504 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/tests/test_ini_parser.py
--rw-r--r--   0 andy       (501) staff       (20)     3682 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/tests/test_larchscore.py
--rw-r--r--   0 andy       (501) staff       (20)      931 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/tests/test_neo_pop.py
--rw-r--r--   0 andy       (501) staff       (20)      338 2024-03-14 06:25:11.000000 exafs_neo-2.0.1/tests/test_utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 04:41:30.471427 exafs_neo-2.0.2/
+-rw-r--r--   0 andy       (501) staff       (20)    35198 2021-08-14 12:28:51.000000 exafs_neo-2.0.2/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)     5897 2024-04-19 04:41:30.471356 exafs_neo-2.0.2/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     5337 2024-04-01 06:56:32.000000 exafs_neo-2.0.2/README.md
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 04:41:30.458792 exafs_neo-2.0.2/exafs_neo/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-02-03 07:16:06.000000 exafs_neo-2.0.2/exafs_neo/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)      152 2024-04-01 06:56:59.000000 exafs_neo-2.0.2/exafs_neo/_version.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 04:41:30.461416 exafs_neo-2.0.2/exafs_neo/analysis/
+-rw-r--r--   0 andy       (501) staff       (20)    28217 2024-04-02 02:45:54.000000 exafs_neo-2.0.2/exafs_neo/analysis/EXAFS_Analysis.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-19 04:33:48.000000 exafs_neo-2.0.2/exafs_neo/analysis/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)    20093 2024-03-19 06:15:52.000000 exafs_neo-2.0.2/exafs_neo/analysis/larch_score.py
+-rw-r--r--   0 andy       (501) staff       (20)     4189 2024-04-02 00:35:24.000000 exafs_neo-2.0.2/exafs_neo/exafs.py
+-rw-r--r--   0 andy       (501) staff       (20)     5812 2024-04-02 02:57:21.000000 exafs_neo-2.0.2/exafs_neo/exafs_pop.py
+-rw-r--r--   0 andy       (501) staff       (20)     5263 2024-04-02 02:59:48.000000 exafs_neo-2.0.2/exafs_neo/exafsfileobj.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 04:41:30.464538 exafs_neo-2.0.2/exafs_neo/gui/
+-rw-r--r--   0 andy       (501) staff       (20)     3079 2024-03-19 04:34:51.000000 exafs_neo-2.0.2/exafs_neo/gui/Analysis_plot.py
+-rw-r--r--   0 andy       (501) staff       (20)     5721 2024-03-18 17:12:48.000000 exafs_neo-2.0.2/exafs_neo/gui/Background_plot.py
+-rw-r--r--   0 andy       (501) staff       (20)     2124 2024-03-18 17:11:48.000000 exafs_neo-2.0.2/exafs_neo/gui/Console.py
+-rw-r--r--   0 andy       (501) staff       (20)     1341 2024-03-18 17:10:04.000000 exafs_neo-2.0.2/exafs_neo/gui/Misc_Function.py
+-rw-r--r--   0 andy       (501) staff       (20)    55561 2024-04-02 19:11:16.000000 exafs_neo-2.0.2/exafs_neo/gui/XAFS_GUI.py
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-18 05:23:32.000000 exafs_neo-2.0.2/exafs_neo/gui/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     3268 2024-03-18 17:10:18.000000 exafs_neo-2.0.2/exafs_neo/gui/feff_folder_larch.py
+-rw-r--r--   0 andy       (501) staff       (20)      265 2023-05-16 01:15:35.000000 exafs_neo-2.0.2/exafs_neo/gui/first_shell_fits.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 04:41:30.466014 exafs_neo-2.0.2/exafs_neo/gui/media/
+-rw-r--r--   0 andy       (501) staff       (20)      539 2023-07-01 21:09:31.000000 exafs_neo-2.0.2/exafs_neo/gui/media/Citation
+-rw-r--r--   0 andy       (501) staff       (20)    35198 2024-04-02 19:10:46.000000 exafs_neo-2.0.2/exafs_neo/gui/media/LICENSE
+-rw-r--r--   0 andy       (501) staff       (20)     3848 2021-08-14 12:28:51.000000 exafs_neo-2.0.2/exafs_neo/gui/media/icon.png
+-rw-r--r--   0 andy       (501) staff       (20)      983 2024-04-02 03:00:16.000000 exafs_neo-2.0.2/exafs_neo/helper.py
+-rw-r--r--   0 andy       (501) staff       (20)     3909 2024-04-02 03:07:35.000000 exafs_neo-2.0.2/exafs_neo/individual.py
+-rw-r--r--   0 andy       (501) staff       (20)     6206 2024-04-02 03:12:20.000000 exafs_neo-2.0.2/exafs_neo/ini_parser.py
+-rwxr-xr-x   0 andy       (501) staff       (20)     1317 2024-04-02 03:13:29.000000 exafs_neo-2.0.2/exafs_neo/input_arg.py
+-rw-r--r--   0 andy       (501) staff       (20)     9228 2024-03-23 23:40:18.000000 exafs_neo-2.0.2/exafs_neo/neoCrossOver.py
+-rw-r--r--   0 andy       (501) staff       (20)     3364 2024-04-02 03:14:48.000000 exafs_neo-2.0.2/exafs_neo/neoFilePars.py
+-rw-r--r--   0 andy       (501) staff       (20)     9223 2024-04-02 03:15:32.000000 exafs_neo-2.0.2/exafs_neo/neoMutator.py
+-rw-r--r--   0 andy       (501) staff       (20)    13651 2024-04-17 06:16:45.000000 exafs_neo-2.0.2/exafs_neo/neoPars.py
+-rw-r--r--   0 andy       (501) staff       (20)     3122 2024-04-02 03:23:54.000000 exafs_neo-2.0.2/exafs_neo/neoResult.py
+-rw-r--r--   0 andy       (501) staff       (20)     3920 2024-04-02 03:27:20.000000 exafs_neo-2.0.2/exafs_neo/neoSelector.py
+-rwxr-xr-x   0 andy       (501) staff       (20)     5748 2024-04-02 05:25:47.000000 exafs_neo-2.0.2/exafs_neo/parser.py
+-rw-r--r--   0 andy       (501) staff       (20)     2953 2024-04-02 05:26:13.000000 exafs_neo-2.0.2/exafs_neo/pathObj.py
+-rw-r--r--   0 andy       (501) staff       (20)     5121 2024-04-02 03:36:53.000000 exafs_neo-2.0.2/exafs_neo/pathrange.py
+-rw-r--r--   0 andy       (501) staff       (20)     1321 2024-04-02 03:39:27.000000 exafs_neo-2.0.2/exafs_neo/pathrange_file.py
+-rw-r--r--   0 andy       (501) staff       (20)    19175 2024-04-02 05:26:30.000000 exafs_neo-2.0.2/exafs_neo/utils.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 04:41:30.471044 exafs_neo-2.0.2/exafs_neo.egg-info/
+-rw-r--r--   0 andy       (501) staff       (20)     5897 2024-04-19 04:41:30.000000 exafs_neo-2.0.2/exafs_neo.egg-info/PKG-INFO
+-rw-r--r--   0 andy       (501) staff       (20)     1482 2024-04-19 04:41:30.000000 exafs_neo-2.0.2/exafs_neo.egg-info/SOURCES.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-04-19 04:41:30.000000 exafs_neo-2.0.2/exafs_neo.egg-info/dependency_links.txt
+-rw-r--r--   0 andy       (501) staff       (20)       99 2024-04-19 04:41:30.000000 exafs_neo-2.0.2/exafs_neo.egg-info/entry_points.txt
+-rw-r--r--   0 andy       (501) staff       (20)        1 2024-02-18 07:51:41.000000 exafs_neo-2.0.2/exafs_neo.egg-info/not-zip-safe
+-rw-r--r--   0 andy       (501) staff       (20)       40 2024-04-19 04:41:30.000000 exafs_neo-2.0.2/exafs_neo.egg-info/requires.txt
+-rw-r--r--   0 andy       (501) staff       (20)       16 2024-04-19 04:41:30.000000 exafs_neo-2.0.2/exafs_neo.egg-info/top_level.txt
+-rw-r--r--   0 andy       (501) staff       (20)       79 2024-04-19 04:41:30.471657 exafs_neo-2.0.2/setup.cfg
+-rw-r--r--   0 andy       (501) staff       (20)     1336 2024-04-19 04:41:27.000000 exafs_neo-2.0.2/setup.py
+drwxr-xr-x   0 andy       (501) staff       (20)        0 2024-04-19 04:41:30.470443 exafs_neo-2.0.2/tests/
+-rw-r--r--   0 andy       (501) staff       (20)        0 2024-03-17 22:01:17.000000 exafs_neo-2.0.2/tests/__init__.py
+-rw-r--r--   0 andy       (501) staff       (20)     4089 2024-03-23 20:03:07.000000 exafs_neo-2.0.2/tests/test_EXAFS_analysis.py
+-rw-r--r--   0 andy       (501) staff       (20)     1607 2024-03-23 19:26:46.000000 exafs_neo-2.0.2/tests/test_exafs_fileobj.py
+-rw-r--r--   0 andy       (501) staff       (20)     3857 2024-03-23 20:01:49.000000 exafs_neo-2.0.2/tests/test_exafs_pars.py
+-rw-r--r--   0 andy       (501) staff       (20)     2280 2024-03-20 02:02:00.000000 exafs_neo-2.0.2/tests/test_exafs_pathObj.py
+-rw-r--r--   0 andy       (501) staff       (20)     1573 2024-02-03 07:05:06.000000 exafs_neo-2.0.2/tests/test_exafs_pathrange.py
+-rw-r--r--   0 andy       (501) staff       (20)     1053 2024-03-20 03:41:05.000000 exafs_neo-2.0.2/tests/test_individual.py
+-rw-r--r--   0 andy       (501) staff       (20)      514 2024-03-17 20:09:18.000000 exafs_neo-2.0.2/tests/test_ini_parser.py
+-rw-r--r--   0 andy       (501) staff       (20)     3385 2024-03-23 20:03:36.000000 exafs_neo-2.0.2/tests/test_larchscore.py
+-rw-r--r--   0 andy       (501) staff       (20)      976 2024-03-23 23:13:20.000000 exafs_neo-2.0.2/tests/test_neo_pop.py
+-rw-r--r--   0 andy       (501) staff       (20)     5754 2024-03-31 00:14:43.000000 exafs_neo-2.0.2/tests/test_neocrossover.py
+-rw-r--r--   0 andy       (501) staff       (20)     3771 2024-04-03 00:18:39.000000 exafs_neo-2.0.2/tests/test_neomutator.py
+-rw-r--r--   0 andy       (501) staff       (20)      338 2024-02-18 20:02:49.000000 exafs_neo-2.0.2/tests/test_utils.py
```

### Comparing `exafs_neo-2.0.1/LICENSE` & `exafs_neo-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.1/PKG-INFO` & `exafs_neo-2.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,109 +1,113 @@
-Metadata-Version: 2.1
-Name: exafs_neo
-Version: 2.0.1
-Summary: exafs_neo AI analysis using GA
-Home-page: https://github.com/laumiulun/EXAFS_Neo
-Download-URL: https://github.com/laumiulun/EXAFS_Neo/tarball/master
-Author: Miu Lun Lau, Jeff Terry, Min Long
-Author-email: andylau@u.boisestate.edu, jterry98@iit.edu, minlong@boisestate.edu
-License: GPLv3
-Keywords: exafs_neo,AI,analysis
-License-File: LICENSE
-
 # EXAFS Neo
 
-#### Versions: 2.0.0
+#### Versions: 2.0.2
 
-#### Last update: Mar 22, 2021
+#### Last update: Mar 23, 2024
 
 <!-- ![example workflow](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/<WORKFLOW_FILE>/badge.svg) -->
 
-[![Test with Ubuntu, Miniconda](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=unit_tests)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Miniconda](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=unit_tests)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
+[![Test with Ubuntu, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
+
 
 EXAFS Neo utilize Genetic algorithm in fitting Extended X-ray absorption fine structure(EXAFS).
 
 ## Prerequisites
 
 It is highly recommend to utilize `anaconda` or `pip` package managers to prevent unforeseen dependency conflicts. EXAFS Neo uses [`larch`](https://xraypy.github.io/xraylarch/) to process the x-ray spectrum.
 
 - Python: => 3.9
 - Numpy: => 1.20
 - Scipy: => 1.6
 - Larch: > 0.9.47
 - Matplotlib: > 3.0
 
-It is highly recommend to create a new environment in `anaconda` to run EXAFS Neo to prevent packages conflicts. For `Windows` operating system, if you encounter a issue requiring "Microsoft C++ 14.0 or greater is needed", please download the tools at the following location [`C++ Tools`](https://visualstudio.microsoft.com/visual-cpp-build-tools/) and make sure to select C++ build tools during installation process.
+It is highly recommend to create a new environment in `anaconda` to run EXAFS Neo to prevent packages conflicts. For `Windows` operating system, if you encounter an issue requiring "Microsoft C++ 14.0 or greater is needed", please download the tools at the following location [`C++ Tools`](https://visualstudio.microsoft.com/visual-cpp-build-tools/) and make sure to select C++ build tools during installation process.
 
 if you are on a Mac (either Intel or M1), you need to make sure that xcode command line tools is install, if not input this command into terminal:
 
         xcode-select --install
 
 ## Dependencies
 
 EXAFS Neo requires the following dependencies to run:
 
         # Create new anaconda environment
         conda create -y --name exafs python=>3.9.10
         conda activate exafs
-        conda install -y "numpy=>1.20" "scipy=>1.6" "matplotlib=>3.0" scikit-learn pandas
-        conda install -y -c conda-forge wxpython pymatgen tomopy pycifrw
+        conda install -y -c conda-forge "numpy>=1.23" "scipy>=1.8" "matplotlib>=3.6" "h5py>=3.5" "wxpython>=4.1" scikit-image scikit-learn pycifrw pandas jupyter plotly pyparsing pytest pytest-cov coverage
+        pip install lmfit peakutils pyepics pyshortcuts termcolor sphinx dill pycifrw xraydb wxmplot wxutils fabio silx imageio charset-normalizer
         pip install xraylarch
 
 ## Installations
 
 To install EXAFS Neo, simply clone the repo:
 
         git clone https://github.com/laumiulun/EXAFS_Neo.git
         cd EXAFS_Neo/
         pip install .
 
 ## Usage
 
-To run a sample test, make sure the environment is set correctly, and select a input file:
+To run the included test suite, use the following command:
+
+        ./run_tests
+
+To run a sample test, make sure the environment is set correctly, and select an input file:
 
          exafs_neo -i test_inputs/test_temp.ini
 
 Alternatively, you can also run EXAFS Neo in a jupyter notebook, please follow the example in the example/jupyter folder
 
-The datafile requires header contain at least either a combination of (k, chi) or (energy, mu). It also requires a minimum of one newline for it to work correctly. An example of the correct header is as follow:
+## GUI
+
+We also have provided a GUI for use in additions to our program, with additional helper script to facilitate post-analysis. To use the GUI:
+
+        exafs_neo_gui
+
+The datafile requires header contain at least either a combination of (k, chi) or (energy, mu). It also requires a minimum of one newline for it to work correctly. An example of the correct header is as follows:
 
         #---------------------------------------------------------------------
         #  k chi chik chik2 chik3 win energy
 
 ## Self adsorption correction
 
-EXAFS also provides a internal option to perform self-adsorption on the sample file using Booth et al correction. This is performed using git submodules:
+EXAFS also provides an internal option to perform self-adsorption on the sample file using Booth et al. correction. This is performed using git submodules:
 
         git submodule update --init --recursive
         cd contrib/sabcor/
         make
 
 ## Update
 
 EXAFS Neo is under active development, to update the code after pulling from the repository:
 
         git pull --rebase
         python setup.py install
 
-## GUI
-
-We also have provided a GUI for use in additions to our program, with additional helper script to facilitate post-analysis. To use the GUI:
 
-        cd gui/
-        python XAFS_GUI.py
 
 ## Video Demonstrations
 
 You can see a list of video demonstrations of the EXAFS Neo package presented, future presentation related to this software will be posted as they are available
 
-<!-- - https://www.youtube.com/playlist?list=PLqZCvArs4yF8IrREQ3AzZJX2N-IRAPEmy [Aug 23,2021] (IIT EXAFS Workshop 2021)
+<!-- - https://www.youtube.com/playlist?list=PLqZCvArs4yF8IrREQ3AzZJX2N-IRAPEmy [Aug 23, 2021] (IIT EXAFS Workshop 2021)
 - https://youtu.be/KwhItvwhapg [Feb 15, 2021] (University of Washington)
 - https://youtu.be/jqISqq_FFR8 [Dec 10, 2020] (Canadian Light Source) -->
 
-- [IIT EXAFS Workshop 2021](https://www.youtube.com/playlist?list=PLqZCvArs4yF8IrREQ3AzZJX2N-IRAPEmy) (Aug 23,2021)
+- [IIT EXAFS Workshop 2021](https://www.youtube.com/playlist?list=PLqZCvArs4yF8IrREQ3AzZJX2N-IRAPEmy) (Aug 23, 2021)
 - [University of Washington](https://youtu.be/KwhItvwhapg) (Feb 15, 2021)
 - [Canadian Light Source](https://youtu.be/jqISqq_FFR8) (Dec 10, 2020)
 
 ## Citation
 
 Jeff Terry, Miu Lun Lau, Jiateng Sun, Chang Xu, Bryan Hendricks, Julia Kise, Mrinalini Lnu, Sanchayni Bagade, Shail Shah, Priyanka Makhijani, Adithya Karantha, Travis Boltz, Max Oellien, Matthew Adas, Shlomo Argamon, Min Long, and Donna Post Guillen, “Analysis of Extended X-ray Absorption Fine Structure (EXAFS) Data Using Artificial Intelligence Techniques,” Applied Surface Science 547, 149059 <https://doi.org/10.1016/j.apsusc.2021.149059> (2021).
+
+    @article{terry2021analysis,
+      title={Analysis of extended X-ray absorption fine structure (EXAFS) data using artificial intelligence techniques},
+      author={Terry, Jeff and Lau, Miu Lun and Sun, Jiateng and Xu, Chang and Hendricks, Bryan and Kise, Julia and Lnu, Mrinalini and Bagade, Sanchayni and Shah, Shail and Makhijani, Priyanka and others},
+      journal={Applied Surface Science},
+      volume={547},
+      pages={149059},
+      year={2021},
+      publisher={Elsevier}
+    }
```

### Comparing `exafs_neo-2.0.1/README.md` & `exafs_neo-2.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,131 @@
+Metadata-Version: 2.1
+Name: exafs_neo
+Version: 2.0.2
+Summary: exafs_neo AI analysis using GA
+Home-page: https://github.com/laumiulun/EXAFS_Neo
+Download-URL: https://github.com/laumiulun/EXAFS_Neo/tarball/master
+Author: Miu Lun Lau, Jeff Terry, Min Long
+Author-email: andylau@u.boisestate.edu, jterry98@iit.edu, minlong@boisestate.edu
+License: GPLv3
+Keywords: exafs_neo,AI,analysis
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: xraylarch
+Requires-Dist: attrs
+Requires-Dist: matplotlib
+Requires-Dist: psutil
+
 # EXAFS Neo
 
-#### Versions: 2.0.0
+#### Versions: 2.0.2
 
-#### Last update: Mar 22, 2021
+#### Last update: Mar 23, 2024
 
 <!-- ![example workflow](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/<WORKFLOW_FILE>/badge.svg) -->
 
-[![Test with Ubuntu, Miniconda](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=unit_tests)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Miniconda](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=unit_tests)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
+[![Test with Ubuntu, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
+
 
 EXAFS Neo utilize Genetic algorithm in fitting Extended X-ray absorption fine structure(EXAFS).
 
 ## Prerequisites
 
 It is highly recommend to utilize `anaconda` or `pip` package managers to prevent unforeseen dependency conflicts. EXAFS Neo uses [`larch`](https://xraypy.github.io/xraylarch/) to process the x-ray spectrum.
 
 - Python: => 3.9
 - Numpy: => 1.20
 - Scipy: => 1.6
 - Larch: > 0.9.47
 - Matplotlib: > 3.0
 
-It is highly recommend to create a new environment in `anaconda` to run EXAFS Neo to prevent packages conflicts. For `Windows` operating system, if you encounter a issue requiring "Microsoft C++ 14.0 or greater is needed", please download the tools at the following location [`C++ Tools`](https://visualstudio.microsoft.com/visual-cpp-build-tools/) and make sure to select C++ build tools during installation process.
+It is highly recommend to create a new environment in `anaconda` to run EXAFS Neo to prevent packages conflicts. For `Windows` operating system, if you encounter an issue requiring "Microsoft C++ 14.0 or greater is needed", please download the tools at the following location [`C++ Tools`](https://visualstudio.microsoft.com/visual-cpp-build-tools/) and make sure to select C++ build tools during installation process.
 
 if you are on a Mac (either Intel or M1), you need to make sure that xcode command line tools is install, if not input this command into terminal:
 
         xcode-select --install
 
 ## Dependencies
 
 EXAFS Neo requires the following dependencies to run:
 
         # Create new anaconda environment
         conda create -y --name exafs python=>3.9.10
         conda activate exafs
-        conda install -y "numpy=>1.20" "scipy=>1.6" "matplotlib=>3.0" scikit-learn pandas
-        conda install -y -c conda-forge wxpython pymatgen tomopy pycifrw
+        conda install -y -c conda-forge "numpy>=1.23" "scipy>=1.8" "matplotlib>=3.6" "h5py>=3.5" "wxpython>=4.1" scikit-image scikit-learn pycifrw pandas jupyter plotly pyparsing pytest pytest-cov coverage
+        pip install lmfit peakutils pyepics pyshortcuts termcolor sphinx dill pycifrw xraydb wxmplot wxutils fabio silx imageio charset-normalizer
         pip install xraylarch
 
 ## Installations
 
 To install EXAFS Neo, simply clone the repo:
 
         git clone https://github.com/laumiulun/EXAFS_Neo.git
         cd EXAFS_Neo/
         pip install .
 
 ## Usage
 
-To run a sample test, make sure the environment is set correctly, and select a input file:
+To run the included test suite, use the following command:
+
+        ./run_tests
+
+To run a sample test, make sure the environment is set correctly, and select an input file:
 
          exafs_neo -i test_inputs/test_temp.ini
 
 Alternatively, you can also run EXAFS Neo in a jupyter notebook, please follow the example in the example/jupyter folder
 
-The datafile requires header contain at least either a combination of (k, chi) or (energy, mu). It also requires a minimum of one newline for it to work correctly. An example of the correct header is as follow:
+## GUI
+
+We also have provided a GUI for use in additions to our program, with additional helper script to facilitate post-analysis. To use the GUI:
+
+        exafs_neo_gui
+
+The datafile requires header contain at least either a combination of (k, chi) or (energy, mu). It also requires a minimum of one newline for it to work correctly. An example of the correct header is as follows:
 
         #---------------------------------------------------------------------
         #  k chi chik chik2 chik3 win energy
 
 ## Self adsorption correction
 
-EXAFS also provides a internal option to perform self-adsorption on the sample file using Booth et al correction. This is performed using git submodules:
+EXAFS also provides an internal option to perform self-adsorption on the sample file using Booth et al. correction. This is performed using git submodules:
 
         git submodule update --init --recursive
         cd contrib/sabcor/
         make
 
 ## Update
 
 EXAFS Neo is under active development, to update the code after pulling from the repository:
 
         git pull --rebase
         python setup.py install
 
-## GUI
-
-We also have provided a GUI for use in additions to our program, with additional helper script to facilitate post-analysis. To use the GUI:
 
-        cd gui/
-        python XAFS_GUI.py
 
 ## Video Demonstrations
 
 You can see a list of video demonstrations of the EXAFS Neo package presented, future presentation related to this software will be posted as they are available
 
-<!-- - https://www.youtube.com/playlist?list=PLqZCvArs4yF8IrREQ3AzZJX2N-IRAPEmy [Aug 23,2021] (IIT EXAFS Workshop 2021)
+<!-- - https://www.youtube.com/playlist?list=PLqZCvArs4yF8IrREQ3AzZJX2N-IRAPEmy [Aug 23, 2021] (IIT EXAFS Workshop 2021)
 - https://youtu.be/KwhItvwhapg [Feb 15, 2021] (University of Washington)
 - https://youtu.be/jqISqq_FFR8 [Dec 10, 2020] (Canadian Light Source) -->
 
-- [IIT EXAFS Workshop 2021](https://www.youtube.com/playlist?list=PLqZCvArs4yF8IrREQ3AzZJX2N-IRAPEmy) (Aug 23,2021)
+- [IIT EXAFS Workshop 2021](https://www.youtube.com/playlist?list=PLqZCvArs4yF8IrREQ3AzZJX2N-IRAPEmy) (Aug 23, 2021)
 - [University of Washington](https://youtu.be/KwhItvwhapg) (Feb 15, 2021)
 - [Canadian Light Source](https://youtu.be/jqISqq_FFR8) (Dec 10, 2020)
 
 ## Citation
 
 Jeff Terry, Miu Lun Lau, Jiateng Sun, Chang Xu, Bryan Hendricks, Julia Kise, Mrinalini Lnu, Sanchayni Bagade, Shail Shah, Priyanka Makhijani, Adithya Karantha, Travis Boltz, Max Oellien, Matthew Adas, Shlomo Argamon, Min Long, and Donna Post Guillen, “Analysis of Extended X-ray Absorption Fine Structure (EXAFS) Data Using Artificial Intelligence Techniques,” Applied Surface Science 547, 149059 <https://doi.org/10.1016/j.apsusc.2021.149059> (2021).
+
+    @article{terry2021analysis,
+      title={Analysis of extended X-ray absorption fine structure (EXAFS) data using artificial intelligence techniques},
+      author={Terry, Jeff and Lau, Miu Lun and Sun, Jiateng and Xu, Chang and Hendricks, Bryan and Kise, Julia and Lnu, Mrinalini and Bagade, Sanchayni and Shah, Shail and Makhijani, Priyanka and others},
+      journal={Applied Surface Science},
+      volume={547},
+      pages={149059},
+      year={2021},
+      publisher={Elsevier}
+    }
```

### Comparing `exafs_neo-2.0.1/exafs_neo/exafs.py` & `exafs_neo-2.0.2/exafs_neo/exafs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import os
+
 from exafs_neo.neoMutator import NeoMutator
 from exafs_neo.exafs_pop import NeoPopulations
 from exafs_neo.neoPars import NeoPars
 from exafs_neo.helper import banner
 from exafs_neo.utils import NeoLogger, STRColors
 from exafs_neo.neoCrossOver import NeoCrossover
 from exafs_neo.neoSelector import NeoSelector
 from exafs_neo.neoResult import NeoResult
+from exafs_neo.ini_parser import validate_input_file
+from exafs_neo.parser import InputParamsParser
 
 
 class ExafsNeo:
 
     def __init__(self, verbose_lvl=5):
         """
         Initialize Params:
@@ -21,37 +25,53 @@
         self.exafs_neo_pars = NeoPars()
         self.mutator = NeoMutator(logger=self.logger)
         self.selector = NeoSelector(logger=self.logger)
         self.crossOver = NeoCrossover(logger=self.logger)
         self.neo_population = None
         self.verbose_lvl = verbose_lvl
         self.result = NeoResult(logger=self.logger)
+        self.input_parameters = None
 
-    def exafs_setup(self, input_parameters):
+    def exafs_read(self, filepath=None, input_parameters=None):
+        """
+        Read the input file into exafs parameters
+        @param str filepath: file path to the ini file
+        @param dict input_parameters: Dictionary of input parameters
+        """
+        if filepath is not None:
+            file_path = os.path.join(os.getcwd(), filepath)
+            input_params = InputParamsParser()
+            input_params.read_input_file(file_path, verbose=False)
+            input_params.input_dict = validate_input_file(input_params.input_dict)
+
+            self.input_parameters = input_params.export_input_dict()
+
+        if input_parameters is not None:
+            self.input_parameters = input_parameters
+
+        if self.input_parameters is None:
+            raise ValueError("No input parameters are given")
+
+    def exafs_setup(self):
         """
         Setup EXAFS run subroutine
-        :param input_parameters: Input parameters of dictionary
         :return:
         """
-
         # TODO:
         #  1. At mid point, do a E0 optimization
-        # self.logger(banner())
-        self.exafs_neo_pars.read_inputs(input_parameters)
+        self.exafs_neo_pars.read_inputs(self.input_parameters)
         self.logger.initialize_logging(self.exafs_neo_pars.neoFilePars.log_path)
         self.neo_population = NeoPopulations(self.exafs_neo_pars)
         self.neo_population.initialize_populations()
         self.result.initialize(self.exafs_neo_pars)
         # Initialize all the operators
         self.selector.initialize(self.exafs_neo_pars)
         self.crossOver.initialize(self.exafs_neo_pars)
         self.mutator.initialize(self.exafs_neo_pars)
 
-        # self.initialize_number()
-
     def run(self):
         """
         Initialize a EXAFS Run
         :return: result class 
         """
         STRColors.run_verbose_start(self.logger, self.exafs_neo_pars, verbose_lvl=self.verbose_lvl)
```

### Comparing `exafs_neo-2.0.1/exafs_neo/exafs_fileobj.py` & `exafs_neo-2.0.2/exafs_neo/exafsfileobj.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import os
 import subprocess
 
-from utils import checkKey, check_if_exists
+from exafs_neo.utils import checkKey, check_if_exists
 
 
 def check_output_files(file):
     """
     Check if the output file for each file exists, else, assumes equality.
 
     Checks:
@@ -32,15 +32,15 @@
     check_if_exists(file_gen)
 
 
 def sabcor_executable(base, sabcorFile, data_path, logger=None):
     """
     Call the sabcor executable from the submodules
 
-    The sabcor exectuable is as follow:
+    The sabcor exectuable is as follows:
 
     sabcor <file.test> <inp>
 
     if input file is <file.test>, output is <file_sac.test>
 
     """
 
@@ -56,15 +56,15 @@
                             stdout=subprocess.PIPE)
         if p == 0:
             if logger != None:
                 logger.print('Sabcor Finished')
             return os.path.splitext(data_path)[0] + "_sac.csv"
 
 
-class exafs_fileobj:
+class ExafsFileobj:
     sabcorFile: str
 
     def __init__(self):
         self.sabcor_toggle = None
         self.end = None
         self.base = None
         self._front = None
@@ -73,24 +73,32 @@
         self.csv_series = False
         self.feff_file = None
         self.output_file = None
 
         self.data_path = None
         self.output_path = None
         self.log_path = None
-
-    def initialize_filepath(self, data_dict, i=0, firstPass=False, path_optimize=False, logger=None, verbose=False):
         """
-        Initialize file paths for each of the file first
 
         Args:
             i (int, optional): the i-th file. Defaults to 0.
             firstPass (bool, optional): if is the first pass through the dataset. Defaults to False.
             path_optimize (bool, optional): if path optimize. Defaults to False.
         """
+    def initialize_filepath(self, data_dict, i=0, firstPass=False, path_optimize=False, logger=None):
+        """
+        Initialize file paths for each of the file first
+
+        @param dict data_dict:
+        @param int i: the i-th file. Defaults to 0.
+        @param bool firstPass: if is the first pass through the dataset. Defaults to False.
+        @param bool path_optimize: if path optimization
+        @param NeoLogger logger: logger
+        @return:
+        """
         # self.csv_series = csv_series
         self.base = os.getcwd()
 
         self.nComp = checkKey('nComp', data_dict, 1, logger=logger)
         self.data_file = checkKey('data_file', data_dict, logger=logger)
         self.feff_file = checkKey('feff_file', data_dict, logger=logger)
         self.output_file = checkKey('output_file', data_dict, logger=logger)
@@ -129,19 +137,20 @@
             sabcor_executable(self.base,
                               self.sabcorFile,
                               self.data_file,
                               logger=logger)
 
 
 if __name__ == "__main__":
-    exafs_File = exafs_fileobj()
+    exafs_File = ExafsFileobj()
 
     data_dict = {
         "data_file": "path_files/Pu_C/pu3in_t030_sac.chi",
-        "feff_file": "path_files/Pu_C/feff/feff",
+        "feff_file": ["path_files/Pu_C/feff/feff","path_files/Pu_C/feff/feff2"],
         "output_file": "result/test/PuC.csv",
+        "nComp": 2,
         "sabcor_toggle": False
     }
 
     exafs_File.initialize_filepath(data_dict)
 
     print(exafs_File.output_file)
```

### Comparing `exafs_neo-2.0.1/exafs_neo/exafs_pop.py` & `exafs_neo-2.0.2/exafs_neo/exafs_pop.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,19 +40,19 @@
     else:
         return loss
 
 
 @define
 class NeoPopulations:
     exafs_NeoPars: NeoPars = None
-    population: list[Individual] = field(factory=list)
+    population: list = field(factory=list)
     population_sorted: list = field(factory=list)
-    population_score: list[int] = field(factory=list)
-    population_perf: dict[Individual, int] = field(factory=dict)
-    next_population: list[Individual] = field(factory=list)
+    population_score: list = field(factory=list)
+    population_perf: dict = field(factory=dict)
+    next_population: list = field(factory=list)
 
     def generate_individual(self):
         if not self.exafs_NeoPars.runPars.secondHalf:
             e0 = np.random.choice(self.exafs_NeoPars.exafsRangePars.rangeE0)
         else:
             e0 = self.exafs_NeoPars.bestFitPars.bestE0
         ind = Individual(self.exafs_NeoPars.exafsPars.npath,
@@ -73,15 +73,15 @@
 
             population_perf[individual] = temp_score
         if sorting:
             self.population_sorted = sorted(
                 population_perf.items(), key=operator.itemgetter(1), reverse=False)
         if replace:
             # self.currBestFit = list(self.population_sorted[0])
-            self.replace_bestfit()
+            self.__replace_bestfit()
         return score
 
     def initialize_populations(self):
         """
         Initialize populations
         :return:
         """
@@ -89,15 +89,15 @@
             self.population.append(self.generate_individual())
 
         self.eval_population()
 
     def __getitem__(self, item):
         return self.population_sorted[item]
 
-    def replace_bestfit(self):
+    def __replace_bestfit(self):
         self.exafs_NeoPars.bestFitPars.currBestInd = self.population_sorted[0][0]
         self.exafs_NeoPars.bestFitPars.currBestVal = self.population_sorted[0][1]
 
         delta = np.abs(self.exafs_NeoPars.bestFitPars.currBestVal - self.exafs_NeoPars.bestFitPars.globBestVal)
         if delta > 0.01:
             self.exafs_NeoPars.bestFitPars.bestDiff = delta
         else:
```

### Comparing `exafs_neo-2.0.1/exafs_neo/helper.py` & `exafs_neo-2.0.2/exafs_neo/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import time
 import numpy as np
 
 from exafs_neo._version import __version__
 
 
-class bcolors:
+class Bcolors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKGREEN = '\033[92m'
     WARNING = '\033[93m'
     FAIL = '\033[91m'
     ENDC = '\033[0m'
     BOLD = '\033[1m'
     UNDERLINE = '\033[4m'
 
 
-def timecall():
+def time_call():
     return time.time()
 
 
 def str_to_bool(s):
     if s == 'True':
         return True
     elif s == 'False':
```

### Comparing `exafs_neo-2.0.1/exafs_neo/individual.py` & `exafs_neo-2.0.2/exafs_neo/individual.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def __init__(self, npaths, pathDictionary, pathrange_Dict, pathlists, e0, pathName):
         """
         Definition:
             npaths = number of paths
             pathDictionary = <dict> path name, and their corresponding paths.dat
             pathrange_Dict = <list> pathrange_limits
             path_lists = the paths lists (can be 2D depends on number of feff)
-            e0 = qunatum e0 of the individuals
+            e0 = quantum e0 of the individuals
             pathname = the paths identifier
         """
         self.npaths = npaths
         self.path_lists = pathlists
         self.pathname = pathName
         self.Population = []
         self.pathrange_Dict = pathrange_Dict
@@ -30,79 +30,92 @@
 
     def get(self):
         """Get all vars
 
         Returns:
             list of (npaths,4) 2D list
         """
-        Population = []
+        population = []
         for i in range(self.npaths):
-            Population.append(self.Population[i].get())
-        return Population
+            population.append(self.Population[i].get())
+        return population
 
     def get_var(self):
         """Get all parameters except e0
 
         Returns:
             list of (npaths,3) 2D list
         """
-        Population = []
+        population = []
         for i in range(self.npaths):
-            Population.append(self.Population[i].get_var())
-        return Population
+            population.append(self.Population[i].get_var())
+        return population
 
     def get_e0(self):
         """Get e0 of the individual
         Returns:
             int: e0 value
         """
         return self.Population[0].get_e0()
 
     def get_path(self, i):
         return self.Population[i].get()
 
     def verbose(self):
         """
-        Print out the Populations
+        Print out the populations
         """
         for i in range(self.npaths):
             self.Population[i].verbose()
 
     def set_path(self, i, s02, sigma2, deltaR):
+        """
+        Set the specfic i-th paths
+        @param int i: index of the paths
+        @param float s02: s02 value
+        @param float sigma2: sigma2 value
+        @param float deltaR: deltaR value
+        @return:
+        """
         self.Population[i].set(s02, sigma2, deltaR)
 
     def set_allpath(self, pars_Arr):
-        """_summary_
-
-        Args:
-            pars_Arr (_type_): _description_
+        """Set the paths of all array given a input array
+        @param np.array pars_Arr: numpy array containing all the paths parameters in (n_path,3)
         """
         assert pars_Arr.shape[0] == self.npaths
         assert pars_Arr.shape[1] == 3
 
         for i in range(self.npaths):
             self.Population[i].set(i, pars_Arr[i][0], pars_Arr[i][1], pars_Arr[i][2])
 
     def set_e0(self, e0):
         """
-        set e0 to a value
-
-        TODO: need to add checker to make sure it valid
+        Set e0 to a value
+        @param float e0: value of e0
+        @return:
         """
         for i in range(self.npaths):
             self.Population[i].set_e0(e0)
 
     def mutate_paths(self, chance):
         """
         Mutate Paths based on the input chance.
+        @param float chance:
+        @return:
         """
         for path in self.Population:
             path.mutate(chance)
 
     def verbose_yTotal(self, intervalk):
+        """
+        return the y total spectrum
+        @param intervalk:
+        @return:
+        """
         yTotal = [0] * (401)
         for i in range(self.npaths):
 
             path = self.pathDictionary.get(self.pathname[i])
             Individual = self.get()
             path.e0 = Individual[i][1]
             path.s02 = Individual[i][0]
```

### Comparing `exafs_neo-2.0.1/exafs_neo/ini_parser.py` & `exafs_neo-2.0.2/exafs_neo/ini_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,32 @@
 """
 Author: Andy Lau
 Last Updated: 1/19/2021
 
 Changes:
 
 2/8/2021: Andy:
-    - Function defintion for arr to be in 2D
+    - Function definition for arr to be in 2D
 
 1/20/2021: Andy:
     - Function definition for optional parameters.
     - Changes to allows for multiple inputs folder.
 
 """
 
 
 def split_path_arr(arr_str, num_compounds):
     """
     Read the path list
+
+    @param str arr_str: str of array for the path list
+    @param int num_compounds: number of compounds
+    @return:
     """
+
     starter = []
     end = []
     k = 0
     split_str = []
     for i in arr_str:
         if i == '[':
             starter.append(k)
@@ -34,28 +39,32 @@
     assert (len(starter) == len(end)), 'Bracket setup not right.'
     if num_compounds > 1:
         assert (num_compounds == len(starter)), 'Number of compounds not matched.'
         assert (num_compounds == len(end)), 'Number of compounds not matched.'
 
     # check if both are zeros, therefore the array is one 1 dimensions
     if len(starter) == 0 and len(end) == 0:
-        # print("1D array only")
         split_str = list(arr_str.split(","))
     else:
-        # # print("2D array")
         for i in range(len(starter)):
             split_str.append(arr_str[starter[i] + 1:end[i]].split(","))
 
     return split_str
 
 
 def optional_var(input_dict, name_var, alt_var=None, type_var=int, output_var=True):
-    """
-    Detections of optional variables exists within input files, and put in corresponding default inputs parameters.
+    """Detections of optional variables exists within input files, and put in corresponding default inputs parameters.
     boolean needs special attentions
+
+    @param dict input_dict: input dictionary
+    @param str name_var: name of the variable
+    @param str alt_var: alternative of the variable
+    @param type type_var: default type of the variable
+    @param str output_var: type of variable.
+    @return:
     """
     if type_var == bool:
         if name_var in input_dict:
             return_var = str_to_bool(input_dict[name_var])
         else:
             return_var = alt_var
     elif type_var is None:
```

### Comparing `exafs_neo-2.0.1/exafs_neo/input_arg.py` & `exafs_neo-2.0.2/exafs_neo/input_arg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import os
 import sys
 
 from exafs_neo.exafs import ExafsNeo
 from exafs_neo.ini_parser import validate_input_file
 from exafs_neo.parser import InputParamsParser
+from exafs_neo._version import __version__
 
 parser = argparse.ArgumentParser()
 
 parser.add_argument('-i', '--input', help="Submit input file to EXAFS")
 parser.add_argument("-v", "--verbose", help="output verbosity", action="store_true")
 parser.add_argument("-s", "--show_input", help="show input file", action="store_true")
 parser.add_argument("-t", help="Timeing mode", action="store_true")
@@ -17,26 +18,26 @@
 args = parser.parse_args()
 if len(sys.argv) == 1:
     parser.print_help(sys.stderr)
     sys.exit(1)
 
 if args.input is not None:
     file_path = os.path.join(os.getcwd(), args.input)
+    print(f"EXAFS Neo {__version__}")
     input_params = InputParamsParser()
     input_params.read_input_file(file_path, verbose=args.show_input)
     input_params.input_dict = validate_input_file(input_params.input_dict)
 
     input_pars = input_params.export_input_dict()
 
-    # print(input_pars)
-
 else:
     print("No input file is given")
 
 debug_mode = args.d
 timeing_mode = args.t
 
 
 def main():
     exafs_neo = ExafsNeo()
-    exafs_neo.exafs_setup(input_pars)
-    result = exafs_neo.run()
+    exafs_neo.exafs_read(input_parameters=input_pars)
+    exafs_neo.exafs_setup()
+    exafs_neo.run()
```

### Comparing `exafs_neo-2.0.1/exafs_neo/neoCrossOver.py` & `exafs_neo-2.0.2/exafs_neo/neoCrossOver.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
 from exafs_neo.exafs_pop import NeoPopulations
 from exafs_neo.neoPars import NeoPars
 
 
 class EXAFS_CrossoverBase:
-    def __init__(self, exafs_pars, logger):
+    def __init__(self, exafs_pars, logger=None):
         self.logger = logger
         self.exafs_pars = exafs_pars
         self.croOpt = self.exafs_pars.crossPars.croOpt
         self.croType = None
 
     def crossover(self, pops, individual1, individual2):
         pass
@@ -49,28 +49,49 @@
 
 class EXAFS_SinglePointCrossover(EXAFS_CrossoverBase):
     def __init__(self, exafs_pars, logger):
         super().__init__(exafs_pars, logger)
         self.croOpt = 1
         self.croType = 'Single Point Crossover'
 
-    def crossover(self, pops, individual1, individual2):
-        pass
+    def crossover(self, pops, individual1, individual2, co_point=1):
+        # prevent overflow by clipping to 0 and 3 for the path
+        co_point = np.clip(co_point, 0, 3)
+        child = pops.generate_individual()
+
+        if np.random.randint(0, 1):
+            child.set_e0(individual1.get_e0())
+        else:
+            child.set_e0(individual2.get_e0())
+
+        for i in range(self.exafs_pars.exafsPathPars.npaths):
+            individual1_path = individual1.get_path(i)
+            individual2_path = individual2.get_path(i)
+
+            temp_path = []
+            for j in range(4):
+                if j < co_point:
+                    temp_path.append(individual1_path[j])
+                else:
+                    temp_path.append(individual2_path[j])
+
+            child.set_path(i, temp_path[0], temp_path[2], temp_path[3])
+
+        return child
 
 
 class EXAFS_DualPointCrossover(EXAFS_CrossoverBase):
     def __init__(self, exafs_pars, logger):
         super().__init__(exafs_pars, logger)
         self.croOpt = 2
         self.croType = 'Dual Point Crossover'
 
     def crossover(self, pops, individual1, individual2):
         pass
 
-
 class EXAFS_ArithmeticCrossover(EXAFS_CrossoverBase):
     def __init__(self, exafs_pars, logger):
         super().__init__(exafs_pars, logger)
         self.croOpt = 3
         self.croType = 'Arithmetic Crossover'
 
     def crossover(self, pops, individual1, individual2):
@@ -125,14 +146,40 @@
                     temp_path.append(individual2_path[j])
 
             child.set_path(i, temp_path[0], temp_path[2], temp_path[3])
 
         return child
 
 
+class EXAFS_AverageCrossOver(EXAFS_CrossoverBase):
+    def __init__(self, exafs_pars, logger):
+        super().__init__(exafs_pars, logger)
+        self.croOpt = 5
+        self.croType = 'Average Crossover'
+
+    def crossover(self, pops, individual1, individual2):
+        child = pops.generate_individual()
+        if np.random.randint(0, 1):
+            child.set_e0(individual1.get_e0())
+        else:
+            child.set_e0(individual2.get_e0())
+
+        for i in range(self.exafs_pars.exafsPathPars.npaths):
+            individual1_path = individual1.get_path(i)
+            individual2_path = individual2.get_path(i)
+
+            temp_path = []
+            for j in range(4):
+                temp_path.append((individual1_path[j] + individual2_path[j]) / 2)
+
+            # TODO check if this values goes out of bound
+            child.set_path(i, temp_path[0], temp_path[2], temp_path[3])
+
+        return child
+
 class NeoCrossover:
     def __init__(self, logger=None):
         self.logger = logger
         self.exafs_pars = None
         self.crossover_type = None
         self.crossover_operator = None
 
@@ -146,14 +193,16 @@
             self.crossover_operator = EXAFS_SinglePointCrossover(exafs_pars, logger=self.logger)
         elif self.crossover_type == 2:
             self.crossover_operator = EXAFS_DualPointCrossover(exafs_pars, logger=self.logger)
         elif self.crossover_type == 3:
             self.crossover_operator = EXAFS_ArithmeticCrossover(exafs_pars, logger=self.logger)
         elif self.crossover_type == 4:
             self.crossover_operator = EXAFS_OrCrossover(exafs_pars, logger=self.logger)
+        elif self.crossover_type == 5:
+            self.crossover_operator = EXAFS_AverageCrossOver(exafs_pars, logger=self.logger)
         else:
             self.crossover_operator = EXAFS_CrossoverBase(exafs_pars, logger=self.logger)
             raise ValueError("Invalid crossover type, returning standard crossover type.")
 
     def __str__(self):
         if self.crossover_operator is None:
             return "Crossover is not selected"
@@ -172,14 +221,20 @@
                     ind2 = pops.next_population[par_ind[1]]
                     child = self.crossover_operator.crossover(pops, ind1, ind2)
                     temp_population.append(child)
 
                 pops.next_population.extend(temp_population)
                 pops.population = pops.next_population
 
+    def crossover_single(self, pops, ind1, ind2):
+        if self.crossover_operator is None:
+            raise ValueError("Crossover is not initialized")
+        else:
+            return self.crossover_operator.crossover(pops, ind1, ind2)
+
 
 if __name__ == "__main__":
     inputs_pars = {'data_file': '../path_files/Cu/cu_10k.xmu', 'output_file': '',
                    'feff_file': '../path_files/Cu/path_75/feff', 'kmin': 0.95,
                    'kmax': 9.775,
                    'kweight': 3.0, 'pathrange': [1, 2, 3, 4, 5],
                    'deltak': 0.05, 'rbkg': 1.1, 'bkgkw': 1.0, 'bkgkmax': 15.0,
```

### Comparing `exafs_neo-2.0.1/exafs_neo/neoFilePars.py` & `exafs_neo-2.0.2/exafs_neo/neoFilePars.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from dataclasses import dataclass, field
+# from dataclasses import dataclass, field
+from attrs import define, field
+
 from pathlib import Path
 
 from exafs_neo.utils import checkKey
 
 
-@dataclass
+@define
 class NeoFilePars:
     base: str = Path.cwd()
     data_file: str = ''
     output_file: str = ''
-    feff_file: list[str] = field(default_factory=list)
+    feff_file: list = field(factory=list)
     log_file: str = 'test.csv'
 
     firstPass: bool = False
     multi_data_toggle: bool = False
-    multi_data: list[str] = field(default_factory=list)
+    multi_data: list = field(factory=list)
     nComp: int = 1
 
-    front: list = field(default_factory=list)
+    front: list = field(factory=list)
 
     data_path: Path = None
     output_path: Path = None
     log_path: Path = None
 
     pathOptimize: bool = False
     end: str = ".dat"
@@ -40,15 +42,16 @@
         self.output_file = checkKey('output_file', input_dicts, '')
         self.log_file = checkKey('log_file', input_dicts, 'test_log.log')
         self.pathOptimize = checkKey('pathOptimize', input_dicts, False)
 
     def initialize_filepath(self, cycles=0):
         """
         Initialize File Path
-        :return:
+        @param int cycles: the cycles of multiple run
+        @return:
         """
 
         if self.nComp > 1:
             for i in range(self.nComp):
                 self.front.append(self.base / self.feff_file[i])
         else:
             self.front = self.base / self.feff_file
@@ -82,8 +85,7 @@
                    'deltak': 0.05, 'rbkg': 1.1, 'bkgkw': 1.0, 'bkgkmax': 15.0, 'pathOptimize': True}
 
     exafs_NeoPars = NeoFilePars()
 
     exafs_NeoPars.read_inputs(inputs_pars)
     exafs_NeoPars.initialize_filepath()
     print(exafs_NeoPars)
-    # print(exafs_NeoPars.neoFilePars)
```

### Comparing `exafs_neo-2.0.1/exafs_neo/neoMutator.py` & `exafs_neo-2.0.2/exafs_neo/neoMutator.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,17 @@
                 self.exafs_pars.mutPars.mutChance += 0.025
                 self.exafs_pars.mutPars.mutChance = abs(self.exafs_pars.mutPars.mutChance)
             elif (abs(diffCounter) / float(self.exafs_pars.runPars.currGen)) < 0.2:
                 if (self.exafs_pars.mutPars.mutChance - 0.025) > 0:
                     self.exafs_pars.mutPars.mutChance -= 0.025
                     self.exafs_pars.mutPars.mutChance = abs(self.exafs_pars.mutPars.mutChance)
 
+            # Clip between 0 and 100%
+            self.exafs_pars.mutPars.mutChance = np.clip(self.exafs_pars.mutPars.mutChance, 0, 100)
+
         for i, _ in enumerate(pops.population):
             if np.random.random() < self.mutChance:
                 new_ind = pops.generate_individual()
                 pops.population[i] = new_ind
                 self.exafs_pars.mutPars.nmut += 1
 
 
@@ -55,29 +58,35 @@
     def __init__(self, exafs_pars, logger):
         super().__init__(exafs_pars, logger)
         self.mutOpt = 2
 
         self.mutType = "Mutate Per Path"
 
     def mutate(self, pops):
-        for i, _ in enumerate(pops.population):
+        for i, individual in enumerate(pops.population):
             if np.random.random() < self.mutChance:
                 pops.population[i].mutate_paths(self.mutChance)
                 self.exafs_pars.mutPars.nmut += 1
 
 
 class ExafsMutator_PerTrait(ExafsMutatorBase):
     def __init__(self, exafs_pars, logger):
         super().__init__(exafs_pars, logger)
         self.mutOpt = 3
 
         self.mutType = "Mutate Per Trait"
 
     def mutate(self, pops):
-        pass
+        for i, pop in enumerate(pops.population):
+            for j, trait in enumerate(pop):
+                if np.random.random() < self.mutChance:
+                    pass
+
+                    # pops.population[i].mutate_paths(self.mutChance)
+                    # self.exafs_pars.mutPars.nmut += 1
 
 
 class ExafsMutator_Metropolis(ExafsMutatorBase):
     def __init__(self, exafs_pars, logger):
         super().__init__(exafs_pars, logger)
         self.mutOpt = 4
 
@@ -228,11 +237,9 @@
     print(neo_population.population[0].get_var())
 
     # Initialize the mutator
     exafs_mutator = NeoMutator()
     exafs_mutator.initialize(exafs_pars=exafs_NeoPars)
     print(exafs_mutator)
     exafs_mutator.mutate(neo_population)
-    # print(exafs_NeoPars.mutPars.nmut)
     print(neo_population.population[0].get_var())
 
-    # exafs_mutator.mutate()
```

### Comparing `exafs_neo-2.0.1/exafs_neo/neoPars.py` & `exafs_neo-2.0.2/exafs_neo/neoPars.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,46 @@
-from dataclasses import dataclass, field
 
 import larch
+
 larch_version = larch.__version__.split('.')
 if int(larch_version[2]) >= 55:
     # New versions
     from larch import Interpreter
     from larch.io import read_ascii
     from larch.xafs import autobk, feffdat, xftf
 else:
     # Old versions
     from larch_plugins.io import read_ascii
     from larch_plugins.xafs import autobk
     from larch_plugins.xafs import feffdat
     from larch_plugins.xafs import xftf
 
-from attrs import define
-from attrs import field as attrs_field
+from attrs import define, field
 import numpy as np
 
 from exafs_neo.pathrange import Pathrange_limits, read_pathrange_file
-from matplotlib import pyplot as plt
 
 from exafs_neo.neoFilePars import NeoFilePars
-from exafs_neo.utils import checkKey, timecall
+from exafs_neo.utils import checkKey, time_call
 
 
 @define
 class NeoBestFit:
     currBestInd: float = None
     currBestVal: float = np.inf
     globBestInd: float = None
     globBestVal: float = np.inf
 
     bestDiff: float = np.inf
     # diffCounter: int = 0
     bestE0: float = 0
 
-    bestChir_magTotal: np.array = attrs_field(default=np.zeros(326))
-    bestYTotal: np.array = attrs_field(default = np.zeros(326))
+    bestChir_magTotal: np.array = field(default=np.zeros(326))
+    bestYTotal: np.array = field(default=np.zeros(326))
+
 
 @define(kw_only=True, slots=True)
 class NeoFixedPars:
     # Neo Fixed Parameters
 
     nPops: float = 100
     nGen: float = 100
@@ -53,14 +52,16 @@
     DE: bool = False
 
     pathOptimize: bool = False
     pathOptimizePercent: float = 0.01
     pathOptimizeOnly: bool = False
     filter_percentage: float = 0.2
 
+    solver: str = 'GA'
+
     printGraph: bool = True
     debug_mode: bool = False
 
     def read_inputs(self, input_dicts):
         self.nPops = checkKey('nPops', input_dicts, 100)
         self.nGen = checkKey('nGen', input_dicts, 100)
         self.steadyState = checkKey('steadyState', input_dicts, False)
@@ -71,91 +72,94 @@
         self.DE = checkKey('DE', input_dicts, False)
 
         self.pathOptimize = checkKey('pathOptimize', input_dicts, False)
         self.pathOptimizePercent = checkKey('pathOptimizePercent', input_dicts, 0.01)
         self.pathOptimizeOnly = checkKey('pathOptimizeOnly', input_dicts, False)
         self.filter_percentage = checkKey('filter_percentage', input_dicts, 0.2)
 
+        self.solver = checkKey('solver', input_dicts, 'GA')
+
         self.printGraph = checkKey('printGraph', input_dicts, True)
         self.debug_mode = checkKey('debug_mode', input_dicts, False)
 
         if self.printGraph:
             # TODO: Implement this
             # self.fig = plt.figure()
             # self.ax = self.fig.add_subplot(111)
             pass
 
 
-@dataclass
+@define
 class NeoRunPars:
     currGen: int = 1
     time: bool = False
     tt: float = 0
     secondHalf: bool = False
     diffCounter: int = 0
     cycles: int = 0
     currGen_st: float = 0
     currGen_tt: float = 0
     nGen: int = 100
 
     def start_gen(self):
-        self.currGen_st = timecall()
+        self.currGen_st = time_call()
 
     def end_gen(self, neo_population):
         self.currGen += 1
-        self.currGen_tt = timecall() - self.currGen_st
+        self.currGen_tt = time_call() - self.currGen_st
         self.tt += self.currGen_tt
         if self.currGen == int(0.5 * self.nGen) - 1:
             neo_population.optimize_e0()
 
         if self.currGen > int(self.nGen / 2):
             self.secondHalf = True
 
     def read_inputs(self, input_dicts):
         self.nGen = checkKey('nGen', input_dicts, 100)
 
+
 @define
 class NeoMutPars:
     """
     Neo Mutation Parameters
     """
     mutOpt: int = 1
-    mutChance: float = attrs_field(default=0.3)
-    mutChanceE0: float = attrs_field(default=0.3)
+    mutChance: float = field(default=0.3)
+    mutChanceE0: float = field(default=0.3)
     nmut: int = 0
 
     def read_inputs(self, input_dicts):
         self.mutOpt = checkKey('mut_options', input_dicts, 1)
         self.mutChance = checkKey('mutChance', input_dicts, 0.3)
         self.mutChanceE0 = checkKey('mutChanceE0', input_dicts, 0.3)
 
     @mutChance.validator
     def check_mutchance(self, attribute, value):
         if value > 1.0 or value < 0.0:
             raise ValueError("mutChance should be between 0 and 1")
 
 
-@dataclass
+@define
 class NeoCrossPars:
     croOpt: int = 0
 
     def read_inputs(self, input_dicts):
         self.croOpt = checkKey('croOpt', input_dicts, 0)
 
 
-@dataclass
+@define
 class NeoSelPars:
     """
     Neo Selection Parameters
     """
     selOpt: int = 0
     nBestSample: float = 0.3
     nLuckSample: float = 0.2
 
-    parents: list = field(default_factory=list)
+    parents: list = field(factory=list)
     __nPop: int = 0
     nBest: int = 0
     nLuck: int = 0
     nCross: int = 0
 
     def read_inputs(self, input_dicts):
         self.selOpt = checkKey('selOpt', input_dicts, 0)
@@ -164,15 +168,15 @@
         self.__nPop = checkKey('nPops', input_dicts, 100)
         self.nBest = int(self.__nPop * self.nBestSample)
         self.nLuck = int(self.__nPop * self.nLuckSample)
         self.nCross = self.__nPop - self.nBest - self.nLuck
 
 
 class NeoPars:
-    def __init__(self,verbose_lvl=5):
+    def __init__(self, verbose_lvl=5):
         """
         Wrapped all paras together
         """
 
         self.verbose_lvl = verbose_lvl
         self.fixedPars = NeoFixedPars()
         self.runPars = NeoRunPars()
@@ -200,22 +204,22 @@
 
         self.exafsPathPars.initialize()
 
 
 @define
 class EXAFSPathRange:
     pathrange_file: str = ''
-    pathrange_pars: list = attrs_field(default=[])
+    pathrange_pars: list = field(default=[])
     npath: int = 0
 
     # e0, for anything
     # rangeE0: np.array = field(default_factory=(np.linspace(-100, 100, 201) * 0.01))
-    rangeE0: np.array = attrs_field(default=np.linspace(-100, 100, 201) * 0.01)
+    rangeE0: np.array = field(default=np.linspace(-100, 100, 201) * 0.01)
     # Large range B
-    rangeE0_large: np.array = attrs_field(default=np.linspace(-600, 600, 1201) * 0.01)
+    rangeE0_large: np.array = field(default=np.linspace(-600, 600, 1201) * 0.01)
 
     def read_inputs(self, input_dicts, exafs_pars):
         self.npath = exafs_pars.npath
         self.pathrange_file = checkKey('pathrange_file', input_dicts, None)
         # self.pathrange_pars = checkKey('pathrange_pars', input_dicts, [])
         if self.pathrange_file is None:
             for i in range(self.npath):
@@ -244,19 +248,19 @@
     rbkg: float = 0.0
     bkgkw: float = 1.0
     bkgkmax: float = 15.0
 
     small: float = 0.0
     big: float = 0.0
     mid: float = 0.0
-    intervalK: list = field(default_factory=list)
+    intervalK: list = field(factory=list)
 
     individual_paths: bool = False
 
-    pathrange: list = field(default_factory=list)
+    pathrange: list = field(factory=list)
     npath: int = 0
 
     def calculate_pars(self):
         self.small = int(self.kmin / self.dk)
         self.big = int(self.kmax / self.dk)
         self.mid = int(self.big - self.small + 1)
         self.intervalK = np.linspace(self.small, self.big, self.mid)
@@ -273,60 +277,60 @@
 
         self.pathrange = checkKey('pathrange', input_dicts, None)
         self.individual_paths = checkKey('individualOptions', input_dicts, False)
         self.npath = len(self.pathrange)
         self.calculate_pars()
 
 
-@dataclass
+@define
 class EXAFSPath:
-    mylarch = Interpreter()
+    mylarch: str = Interpreter()
     g: larch.symboltable.Group = None
     best: larch.symboltable.Group = None
     sumgroup: larch.symboltable.Group = None
-    exp = None
-    pathname: list = field(default_factory=list)
+    exp: list = field(factory=list)
+    pathname: list = field(factory=list)
     ncomp: int = 0
     individual_paths: bool = False
-    path_lists: list = field(default_factory=list)
-    pathDictionary: dict = field(default_factory=dict)
+    path_lists: list = field(factory=list)
+    pathDictionary: dict = field(factory=dict)
 
     # def initialize(self):
     # self.read_inputs(exafs_neo)
 
-    end = None
-    front = None
-    npaths = None
-    exafs_static_pars = None
-    exafs_file_pars = None
+    end: str = None
+    front: list = field(factory=list)
+    npaths: int = None
+    exafs_static_pars: EXAFSStaticPars = None
+    exafs_file_pars: NeoFilePars = None
 
     def read_inputs(self, exafs_filepars: NeoFilePars, exafs_static_pars: EXAFSStaticPars):
         self.exafs_file_pars = exafs_filepars
         self.exafs_static_pars = exafs_static_pars
         self.g = read_ascii(str(exafs_filepars.data_path))
         self.best = read_ascii(str(exafs_filepars.data_path))
         self.sumgroup = read_ascii(str(exafs_filepars.data_path))
-        self.ncomp = NeoFilePars.nComp
+        self.ncomp = exafs_filepars.nComp
         self.individual_paths = exafs_static_pars.individual_paths
         self.npaths = exafs_static_pars.npath
         self.front = exafs_filepars.front
         self.end = exafs_filepars.end
         self.path_lists = exafs_static_pars.pathrange
 
-    def initialize_group(self):
+    def __initialize_group(self):
         try:
             self.g.k
             self.g.chi
         except AttributeError:
             autobk(self.g, rbkg=self.exafs_static_pars.rbkg, kweight=self.exafs_static_pars.kweight,
                    kmax=self.exafs_static_pars.kmax, _larch=self.mylarch)
             autobk(self.best, rbkg=self.exafs_static_pars.rbkg, _larch=self.mylarch)
             autobk(self.sumgroup, rbkg=self.exafs_static_pars.rbkg, _larch=self.mylarch)
 
-    def initialize_paths(self):
+    def __initialize_paths(self):
         """
         Load paths:
             Initialize paths in various files.
         """
         self.pathname = []
         if self.ncomp > 1:
             if self.individual_paths:
@@ -355,32 +359,32 @@
                 for i in range(1, self.npaths + 1):
                     filename = str(self.front) + str(i).zfill(4) + self.end
                     pathName = f"Path{i}"
                     self.pathname.append(pathName)
                     self.pathDictionary.update(
                         {pathName: feffdat.feffpath(filename, _larch=self.mylarch)})
 
-    def initialize_ftf(self):
+    def __initialize_ftf(self):
         xftf(self.g.k, self.g.chi, kmin=self.exafs_static_pars.kmin, kmax=self.exafs_static_pars.kmax, dk=4,
              window='hanning',
              kweight=self.exafs_static_pars.kweight, group=self.g, _larch=self.mylarch)
         xftf(self.best.k, self.best.chi, kmin=self.exafs_static_pars.kmin, kmax=self.exafs_static_pars.kmax, dk=4,
              window='hanning',
              kweight=self.exafs_static_pars.kweight, group=self.best, _larch=self.mylarch)
         xftf(self.sumgroup.k, self.sumgroup.chi, kmin=self.exafs_static_pars.kmin, kmax=self.exafs_static_pars.kmax,
              dk=4,
              window='hanning',
              kweight=self.exafs_static_pars.kweight, group=self.sumgroup, _larch=self.mylarch)
 
         self.exp = self.g.chi
 
     def initialize(self):
-        self.initialize_group()
-        self.initialize_paths()
-        self.initialize_ftf()
+        self.__initialize_group()
+        self.__initialize_paths()
+        self.__initialize_ftf()
 
 
 if __name__ == "__main__":
     # exafs_pars = EXAFSPars()
     inputs_pars = {'data_file': '../path_files/Cu/cu_10k.xmu', 'output_file': '',
                    'feff_file': '../path_files/Cu/path_75/feff', 'kmin': 0.95,
                    'kmax': 9.775,
```

### Comparing `exafs_neo-2.0.1/exafs_neo/neoResult.py` & `exafs_neo-2.0.2/exafs_neo/neoResult.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,58 +20,77 @@
     def __str__(self):
         if self.best_individual is None:
             return f"Best Individual: None"
         else:
             return f"Best Individual: {self.best_individual}"
 
     def save(self, filename):
+        """
+        Save the Neo Result file
+        :param str filename: file name of the neo result
+        :return:
+        """
+
         try:
             with open(filename, 'wb') as file:
                 pickle.dump(self, file)
         except Exception as e:
             self.logger.print(f"Error saving file: {e}")
 
     @classmethod
     def load(cls, filename):
+        """
+        Load the result file back into it
+        :param str filename: load back the neo object.
+        :return:
+        """
         try:
             with open(filename, 'rb') as file:
                 obj = pickle.load(file)
             print(f"Object loaded from {filename}")
             return obj
         except Exception as e:
             print(f"Error loading object: {e}")
             return None
 
     def initialize(self, exafs_pars):
         self.exafs_pars = exafs_pars
 
     def collect(self, neo_population, exafs_pars):
+        """
+        Collecting all result into a single area for post processing.
+        :param neo_population:
+        :param exafs_pars:
+        :return:
+        """
         self.exafs_pars = exafs_pars
         self.best_individual = neo_population.population_sorted[0][0]
         self.historyBest.append(exafs_pars.bestFitPars.globBestVal)
         global_r = exafs_pars.bestFitPars.globBestVal / (
                 len(exafs_pars.exafsPars.intervalK) - 3 * exafs_pars.exafsPars.npath + 1)
         self.historyBestChiR.append(global_r)
 
     def plot_fitness(self):
+        """
+        Plot the fitness function
+        :return:
+        """
         x = np.arange(0, len(self.historyBest), 1)
 
         fig, ax1 = plt.subplots()
         ax1.plot(x, self.historyBest, 'Fitness')
         ax1.set_xlabel('Generation')
         ax1.set_ylabel('Fitness', color='b')
         # ax1.tick_params('y', colors='b')
         ax1.set_xticks(x)
 
         ax2 = ax1.twinx()
         ax2.plot(x, self.historyBestChiR, 'Fitness Reduced Chi2')
         ax2.set_ylabel('Fitness Reduced Chi2', color='r')
 
-
-
         # locs, labels = plt.xticks()
         # plt.plot(x, self.historyBest, label='Fitness ')
         # # plt.plot(x,self.historyBestChiR,label='Fitness Reduced Chi2')
         # plt.xlabel('Generation')
         # plt.ylabel('Fitness')
         # plt.xticks(x)
```

### Comparing `exafs_neo-2.0.1/exafs_neo/neoSelector.py` & `exafs_neo-2.0.2/exafs_neo/neoSelector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from exafs_neo.exafs_pop import NeoPopulations
 from exafs_neo.neoPars import NeoPars
 
 
 class ExafsSelectorBase:
     def __init__(self, exafs_pars, logger):
+        """
+        Initialize the selector base class
+        :param exafs_pars:
+        :param logger:
+        """
         self.logger = logger
         self.exafs_pars = exafs_pars
         self.npops = exafs_pars.fixedPars.nPops
         self.nBest_Percent = exafs_pars.selPars.nBestSample
         self.nLucky_Percent = exafs_pars.selPars.nLuckSample
 
         self.nBest = int(self.nBest_Percent * self.npops)
@@ -49,32 +54,47 @@
         self.selector_operator = "Tournament"
 
     def select(self, pops):
         pass
 
 
 class NeoSelector:
+
     def __init__(self, logger=None):
+        """
+        Neo Selector
+        :param NeoLogger logger: logger for Neo
+        """
         self.selector_operator = None
         self.logger = logger
         self.selector_type = None
         self.exafs_pars = None
 
     def initialize(self, exafs_pars):
+        """
+        Initialize the Selector
+        :param exafs_pars:
+        :return:
+        """
         self.exafs_pars = exafs_pars
         self.selector_type = exafs_pars.selPars.selOpt
         if self.selector_type == 0:
             self.selector_operator = ExafsSelector_RouletteWheel(exafs_pars, logger=self.logger)
         elif self.selector_type == 1:
             self.selector_operator = ExafsSelector_Tournament(exafs_pars, logger=self.logger)
         else:
             self.selector_operator = ExafsSelectorBase(exafs_pars, logger=self.logger)
             raise ValueError("Invalid selector type, returning standard selector type.")
 
     def select(self, pops):
+        """
+        Perform the actual selection
+        :param NeoPopulation pops:  
+        :return:
+        """
         if self.selector_operator is None:
             raise ValueError("Selector is not initialized")
         else:
             return self.selector_operator.select(pops)
 
     def __str__(self):
         if self.selector_operator is None:
```

### Comparing `exafs_neo-2.0.1/exafs_neo/parser.py` & `exafs_neo-2.0.2/exafs_neo/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # Parser for Inputs files
-import os
 import configparser
 from dataclasses import dataclass, field
 
-from exafs_neo.helper import bcolors
+from exafs_neo.helper import Bcolors
 
 
 def CheckKey(dict, key_list):
     for i in range(len(key_list)):
         try:
             dict[key_list[i]]
         except KeyError:
             raise KeyError(str(key_list[i]) + ' is missing')
             # break
 
 
 def print_input_file(file_dict):
     for key, value in file_dict.items():
-        print("[" + bcolors.BOLD + str(key) + bcolors.ENDC + "]")
+        print("[" + Bcolors.BOLD + str(key) + Bcolors.ENDC + "]")
         for inner_key, inner_value in value.items():
             print('---' + inner_key + ": " + inner_value)
 
 
 def check_optional_key(og_dict, optional_key_list):
     optional_key = []
     for i in range(len(optional_key_list)):
```

### Comparing `exafs_neo-2.0.1/exafs_neo/pathObj.py` & `exafs_neo-2.0.2/exafs_neo/pathObj.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import random
 
 import attr
-from attrs import asdict, define, make_class, Factory
 import numpy as np
 from exafs_neo.pathrange import Pathrange_limits
-from attrs import asdict, define, make_class, Factory
 
 """
 Author: Andy Lau
 
 """
 
 
@@ -42,28 +40,19 @@
     def get(self):
         return [self.s02, self.e0, self.sigma2, self.deltaR]
 
     def get_var(self):
         return [self.s02, self.sigma2, self.deltaR]
 
     def verbose(self):
-        print(self.s02, self.e0, self.sigma2, self.deltaR, ",", self.path)
-
-    def get_s02(self):
-        return self.s02
+        print(self.s02, self.e0, self.sigma2, self.deltaR)
 
     def get_e0(self):
         return self.e0
 
-    def get_sigma2(self):
-        return self.sigma2
-
-    def get_deltaR(self):
-        return self.deltaR
-
     # -----------------
     def set_s02(self, s02):
         self.s02 = s02
 
     def set_e0(self, e0):
         """_summary_
 
@@ -81,33 +70,36 @@
         self.deltaR = deltaR
 
     def set(self, s02, sigma2, deltaR):
         self.set_s02(s02)
         self.set_sigma2(sigma2)
         self.set_deltaR(deltaR)
 
-    def mutate_s02(self, chance):
+    def __mutate_s02(self, chance):
         if random.random() * 100 < chance:
             self.s02 = np.random.choice(self.pathrange_obj.getrange_S02())
 
-    def mutate_sigma2(self, chance):
+    def __mutate_sigma2(self, chance):
         if random.random() * 100 < chance:
             self.sigma2 = np.random.choice(self.pathrange_obj.getrange_Sigma2())
 
-    def mutate_deltaR(self, chance):
+    def __mutate_deltaR(self, chance):
         if random.random() * 100 < chance:
             self.deltaR = np.random.choice(self.pathrange_obj.getrange_DeltaR())
 
     def mutate(self, chance):
         """
         Mutated each of the parameters
+
+        :param float chance: mutation chance
+        :return:
         """
-        self.mutate_s02(chance)
-        self.mutate_sigma2(chance)
-        self.mutate_deltaR(chance)
+        self.__mutate_s02(chance)
+        self.__mutate_sigma2(chance)
+        self.__mutate_deltaR(chance)
 
     def __str__(self):
         return f"PathObject: s02: {np.round(self.s02, 2)}, e0: {np.round(self.e0, 2)}, sigma2: {np.round(self.sigma2, 3)}, deltaR: {np.round(self.deltaR, 4)}"
 
 
 if __name__ == '__main__':
     e0 = 0.37
```

### Comparing `exafs_neo-2.0.1/exafs_neo/pathrange.py` & `exafs_neo-2.0.2/exafs_neo/pathrange.py`

 * *Files 13% similar despite different names*

```diff
@@ -68,27 +68,27 @@
         self.glob_rangeSigma2 = copy.deepcopy(self.rangeSigma2)
         self.glob_rangeDeltaR = copy.deepcopy(self.rangeDeltaR)
 
     def get_lim(self):
         lim_s02 = self.get_lim_S02()
         lim_sigma2 = self.get_lim_Sigma2()
         lim_deltaR = self.get_lim_DeltaR()
-        return (self._path_, lim_s02, lim_sigma2, lim_deltaR)
+        return self._path_, lim_s02, lim_sigma2, lim_deltaR
 
     def get_lim_S02(self):
-        return (self.S02_min, self.S02_max, self.S02_dt)
+        return self.S02_min, self.S02_max, self.S02_dt
 
     def get_lim_Sigma2(self):
-        return (self.Sigma2_min, self.Sigma2_max, self.Sigma2_dt)
+        return self.Sigma2_min, self.Sigma2_max, self.Sigma2_dt
 
     def get_lim_DeltaR(self):
-        return (self.deltaR_min, self.deltaR_max, self.deltaR_dt)
+        return self.deltaR_min, self.deltaR_max, self.deltaR_dt
 
     def get_lim_E0(self):
-        return (-1, 1, 0.01)
+        return -1, 1, 0.01
 
     # Get the range for each specific parameter
     def get_path(self):
         return self._path_
 
     def getrange_S02(self):
         return self.rangeS02
@@ -99,15 +99,15 @@
     def getrange_Sigma2(self):
         return self.rangeSigma2
 
     def getrange_DeltaR(self):
         return self.rangeDeltaR
 
     def getrange(self):
-        return (self.getrange_S02(), self.getrange_E0(), self.getrange_Sigma2(), self.getrange_DeltaR())
+        return self.getrange_S02(), self.getrange_E0(), self.getrange_Sigma2(), self.getrange_DeltaR()
 
     # Modify parameters of each objects
     def mod_range(self, glob_arr, val):
         index = next(i for i, _ in enumerate(glob_arr) if np.isclose(_, val, self._tol))
         lower = index - self.offset_val
         upper = index + self.offset_val
 
@@ -136,18 +136,18 @@
     raise Exception(msg)
 
 
 def check_range(val_low, val_high, delta_val):
     if np.abs(val_high - val_low) / delta_val < 1:
         raise_error('Delta Spacing too high')
     try:
-        range = np.arange(val_low, val_high, delta_val)
+        filtered_range = np.arange(val_low, val_high, delta_val)
     except:
         pass
-    return range
+    return filtered_range
 
 
 def read_pathrange_file(file, num_path):
     # Read in the custom input files
     raw_data = np.genfromtxt(file, delimiter=",")
     raw_npath = raw_data.shape[0]
     if num_path != raw_npath:
```

### Comparing `exafs_neo-2.0.1/exafs_neo/pathrange_file.py` & `exafs_neo-2.0.2/exafs_neo/pathrange_file.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,39 +8,41 @@
 
 # Format:
 Paths,(S02_LOW,S02,HIGH,DELTA_S02),(SIGMA2_LOW,SIGMA2_High,DELTA_SIGMA2),(DELTAR_LOW,DELTAR_High,DELTA_DELTAR)
 
  User can create their own inputs files which corresponds to the
 """
 import numpy as np
+from exafs_neo.utils import raise_error
 
-def raise_error(msg='Error'):
-    raise Exception(msg)
 
-def check_range(val_low,val_high,delta_val):
-    if np.abs(val_high - val_low)/delta_val < 1:
+
+def check_range(val_low, val_high, delta_val):
+    if np.abs(val_high - val_low) / delta_val < 1:
         raise_error('Delta Spacing too high')
     try:
-        range = np.arange(val_low,val_high,delta_val)
+        selected_range = np.arange(val_low, val_high, delta_val)
     except:
         pass
-    return range
+    return selected_range
+
 
-def read_pathrange_file(file,num_path):
+def read_pathrange_file(file, num_path):
     # Read in the custom input files
-    raw_data = np.genfromtxt(file,delimiter=",")
+    raw_data = np.genfromtxt(file, delimiter=",")
     raw_npath = raw_data.shape[0]
     if num_path != raw_npath:
         raise_error("Mismatch in number of paths")
 
     if raw_data.shape[1] != 10:
         raise_error("Number of Columns not right")
     for i in range(num_path):
-        check_range(raw_data[i][1],raw_data[i][2],raw_data[i][3])
-        check_range(raw_data[i][4],raw_data[i][5],raw_data[i][6])
-        check_range(raw_data[i][7],raw_data[i][8],raw_data[i][9])
+        check_range(raw_data[i][1], raw_data[i][2], raw_data[i][3])
+        check_range(raw_data[i][4], raw_data[i][5], raw_data[i][6])
+        check_range(raw_data[i][7], raw_data[i][8], raw_data[i][9])
 
     return raw_data
 
+
 if __name__ == "__main__":
-    file = 'test/test_custom_input.txt'
-    read_pathrange_file(file,5)
+    test_file = 'test/test_custom_input.txt'
+    read_pathrange_file(test_file, 5)
```

### Comparing `exafs_neo-2.0.1/exafs_neo/utils.py` & `exafs_neo-2.0.2/exafs_neo/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import datetime
 import logging
 import pathlib
 import sys
-import time
 
 import numpy as np
-from exafs_neo.helper import banner
+from exafs_neo.helper import time_call
 
 
-# from helper import banner
-def timecall():
-    return time.time()
+def raise_error(msg='Error'):
+    raise Exception(msg)
 
 
 def checkKey(key, dictionary, alt_value=None, logger=None, verbose=False):
     # TODO: Raise checker for alternative response
     if key not in dictionary:
         if verbose:
             warn_str = f'{key} not found! Using default value of {key}: {alt_value}'
@@ -22,14 +20,15 @@
                 print(warn_str)
             else:
                 logger.warn(warn_str)
         return alt_value
     else:
         return dictionary[key]
 
+
 class NeoLogger:
     def __init__(self):
         logging.basicConfig(level=logging.DEBUG)
         self.logger = logging.getLogger('')
         # file_handler = logging.FileHandler()
         if self.logger.hasHandlers():
             self.logger.handlers.clear()
@@ -72,48 +71,14 @@
     pathFile = pathlib.Path(path_file)
     if pathFile.is_file():
         pathFile.unlink()
     # Make Directory when its missing
     pathFile.parent.mkdir(parents=True, exist_ok=True)
 
 
-def check_output_file(file, output_path):
-    """
-    check if the output file for each file, assumes equality.
-    """
-    file_base = pathlib.Path(file).with_suffix('')
-    check_if_exists(file)
-    # self.file = file
-    # Open a empty file
-    file_initial = open(output_path, "a+")
-    # Write header to file
-    file_initial.write(
-        "Gen,TPS,FITTNESS,CO_Score,Mut_Score,CURRFIT,CURRIND,BESTFIT,BESTIND\n")  # writing header
-    file_initial.close()
-
-    # Not using right now
-    """
-    # file_score = os.path.splitext(file)[0] + '_score.csv'
-    # self.check_if_exists(file_score)
-    # self.file_score = file_score
-    """
-    # file_data = os.path.splitext(file)[0] + '_data.csv'
-    file_data = pathlib.Path(str(file_base) + "_data.csv")
-    check_if_exists(file_data)
-    file_data = file_data
-
-    # Not using right now
-    # file_gen = os.path.splitext(file)[0] + '_generations.csv'
-    file_gen = pathlib.Path(str(file_base) + "_generations.csv")
-    check_if_exists(file_gen)
-    # self.file_gen = file_gen
-
-    return file_data, file_gen
-
-
 class STRColors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKGREEN = '\033[92m'
     WARNING = '\033[93m'
     FAIL = '\033[91m'
     ENDC = '\033[0m'
@@ -190,77 +155,146 @@
                                                     f"{STRColors.BOLD}Path Optimize Percent{STRColors.ENDC}: {exafs_NeoPars.fixedPars.pathOptimizePercent}",
                                                     verbose_lvl, 5)
         STRColors.logger_print_based_on_verbose_lvl(logger,
                                                     f"{STRColors.BOLD}Path Optimize Only{STRColors.ENDC}: {exafs_NeoPars.fixedPars.pathOptimizeOnly}",
                                                     verbose_lvl, 5)
         STRColors.logger_print_based_on_verbose_lvl(logger, "----------------Mutations------------------",
                                                     verbose_lvl, 5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Mutations{STRColors.ENDC}: {exafs_NeoPars.mutPars.mutChance}",
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Mutations{STRColors.ENDC}: {exafs_NeoPars.mutPars.mutChance}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}E0 Mutations{STRColors.ENDC}: {exafs_NeoPars.mutPars.mutChanceE0}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Mutation Options{STRColors.ENDC}: {exafs_NeoPars.mutPars.mutOpt}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Selection Options{STRColors.ENDC}: {exafs_NeoPars.selPars.selOpt}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Crossover Options{STRColors.ENDC}: {exafs_NeoPars.crossPars.croOpt}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger, "---------------Larch Paths-----------------", verbose_lvl,
+                                                    5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Kmin{STRColors.ENDC}: {exafs_NeoPars.exafsPars.kmin}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Kmax{STRColors.ENDC}: {exafs_NeoPars.exafsPars.kmax}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Kweight{STRColors.ENDC}: {exafs_NeoPars.exafsPars.kweight}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Delta k{STRColors.ENDC}: {exafs_NeoPars.exafsPars.dk}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}RBKG{STRColors.ENDC}: {exafs_NeoPars.exafsPars.rbkg}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}BKG Kw{STRColors.ENDC}: {exafs_NeoPars.exafsPars.bkgkw}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}BKG Kmax{STRColors.ENDC}: {exafs_NeoPars.exafsPars.bkgkmax}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger, "-------------------------------------------", verbose_lvl,
+                                                    5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Steady State{STRColors.ENDC}: {exafs_NeoPars.fixedPars.steadyState}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Print Graph{STRColors.ENDC}: {exafs_NeoPars.fixedPars.printGraph}",
                                                     verbose_lvl, 5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}E0 Mutations{STRColors.ENDC}: {exafs_NeoPars.mutPars.mutChanceE0}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Mutation Options{STRColors.ENDC}: {exafs_NeoPars.mutPars.mutOpt}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Selection Options{STRColors.ENDC}: {exafs_NeoPars.selPars.selOpt}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Crossover Options{STRColors.ENDC}: {exafs_NeoPars.crossPars.croOpt}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, "---------------Larch Paths-----------------",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Kmin{STRColors.ENDC}: {exafs_NeoPars.exafsPars.kmin}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Kmax{STRColors.ENDC}: {exafs_NeoPars.exafsPars.kmax}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Kweight{STRColors.ENDC}: {exafs_NeoPars.exafsPars.kweight}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Delta k{STRColors.ENDC}: {exafs_NeoPars.exafsPars.dk}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}RBKG{STRColors.ENDC}: {exafs_NeoPars.exafsPars.rbkg}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}BKG Kw{STRColors.ENDC}: {exafs_NeoPars.exafsPars.bkgkw}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}BKG Kmax{STRColors.ENDC}: {exafs_NeoPars.exafsPars.bkgkmax}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, "-------------------------------------------",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Steady State{STRColors.ENDC}: {exafs_NeoPars.fixedPars.steadyState}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Print Graph{STRColors.ENDC}: {exafs_NeoPars.fixedPars.printGraph}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, "-------------------------------------------",verbose_lvl,5)
+        STRColors.logger_print_based_on_verbose_lvl(logger, "-------------------------------------------", verbose_lvl,
+                                                    5)
 
     @staticmethod
     def run_verbose_gen(logger, exafs_NeoPars, neo_population, verbose_lvl=5):
         """
         Verbose generation
         """
-        st = timecall()
+        st = time_call()
         population_sorted = neo_population.population_sorted
-        STRColors.logger_print_based_on_verbose_lvl(logger, "---------------------------------------------------------",verbose_lvl,1)
-        STRColors.logger_print_based_on_verbose_lvl(logger, datetime.datetime.fromtimestamp(st).strftime('%H:%M:%S') + f"{STRColors.BOLD} Gen: {STRColors.ENDC}{exafs_NeoPars.runPars.currGen}",verbose_lvl,1)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"Best Fit: {STRColors.BOLD}{population_sorted[0][1].round(3)}{STRColors.ENDC}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger,  f"Best Fit: {STRColors.BOLD}{population_sorted[0][1].round(3)}{STRColors.ENDC}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger,  f"2nd Fit: {STRColors.BOLD}{population_sorted[1][1].round(3)}{STRColors.ENDC}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger,  f"3rd Fit: {STRColors.BOLD}{population_sorted[2][1].round(3)}{STRColors.ENDC}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger,  f"4th Fit: {STRColors.BOLD}{population_sorted[0][1].round(3)}{STRColors.ENDC}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger,  f"Last Fit: {STRColors.BOLD}{population_sorted[-1][1].round(3)}{STRColors.ENDC}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"Different from last best fit: {exafs_NeoPars.bestFitPars.bestDiff:.4f}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, STRColors.BOLD + "Best fit: " + STRColors.OKBLUE + str(np.round(exafs_NeoPars.bestFitPars.currBestVal, 3)) + STRColors.ENDC,verbose_lvl,5)
-        CurrchiR = np.round(exafs_NeoPars.bestFitPars.currBestVal / (len(exafs_NeoPars.exafsPars.intervalK) - 3 * exafs_NeoPars.exafsPars.npath + 1), 3)
-        STRColors.logger_print_based_on_verbose_lvl(logger, STRColors.BOLD + "Best fit ChiR: " + STRColors.OKBLUE + str(CurrchiR) + STRColors.ENDC,verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, STRColors.BOLD + "History Best: " + STRColors.OKBLUE + str(np.round(exafs_NeoPars.bestFitPars.globBestVal, 4)) + STRColors.ENDC,verbose_lvl,1)
-        GlobchiR = exafs_NeoPars.bestFitPars.globBestVal / (len(exafs_NeoPars.exafsPars.intervalK) - 3 * exafs_NeoPars.exafsPars.npath + 1)
-        STRColors.logger_print_based_on_verbose_lvl(logger, STRColors.BOLD + "History Best ChiR: " + STRColors.OKBLUE + str(np.round(GlobchiR, 4)) + STRColors.ENDC,verbose_lvl,1)
-        STRColors.logger_print_based_on_verbose_lvl(logger, "DiffCounter: " + str(exafs_NeoPars.runPars.diffCounter),verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"Diff %: {(exafs_NeoPars.runPars.diffCounter / exafs_NeoPars.runPars.currGen):.3f}",verbose_lvl,5)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"Mutation Chance: {100 * exafs_NeoPars.mutPars.mutChance:.2f}%",verbose_lvl,5)
+        STRColors.logger_print_based_on_verbose_lvl(logger, "---------------------------------------------------------",
+                                                    verbose_lvl, 1)
+        STRColors.logger_print_based_on_verbose_lvl(logger, datetime.datetime.fromtimestamp(st).strftime(
+            '%H:%M:%S') + f"{STRColors.BOLD} Gen: {STRColors.ENDC}{exafs_NeoPars.runPars.currGen}", verbose_lvl, 1)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"Best Fit: {STRColors.BOLD}{population_sorted[0][1].round(3)}{STRColors.ENDC}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"Best Fit: {STRColors.BOLD}{population_sorted[0][1].round(3)}{STRColors.ENDC}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"2nd Fit: {STRColors.BOLD}{population_sorted[1][1].round(3)}{STRColors.ENDC}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"3rd Fit: {STRColors.BOLD}{population_sorted[2][1].round(3)}{STRColors.ENDC}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"4th Fit: {STRColors.BOLD}{population_sorted[0][1].round(3)}{STRColors.ENDC}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"Last Fit: {STRColors.BOLD}{population_sorted[-1][1].round(3)}{STRColors.ENDC}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"Different from last best fit: {exafs_NeoPars.bestFitPars.bestDiff:.4f}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger, STRColors.BOLD + "Best fit: " + STRColors.OKBLUE + str(
+            np.round(exafs_NeoPars.bestFitPars.currBestVal, 3)) + STRColors.ENDC, verbose_lvl, 5)
+        CurrchiR = np.round(exafs_NeoPars.bestFitPars.currBestVal / (
+                    len(exafs_NeoPars.exafsPars.intervalK) - 3 * exafs_NeoPars.exafsPars.npath + 1), 3)
+        STRColors.logger_print_based_on_verbose_lvl(logger, STRColors.BOLD + "Best fit ChiR: " + STRColors.OKBLUE + str(
+            CurrchiR) + STRColors.ENDC, verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger, STRColors.BOLD + "History Best: " + STRColors.OKBLUE + str(
+            np.round(exafs_NeoPars.bestFitPars.globBestVal, 4)) + STRColors.ENDC, verbose_lvl, 1)
+        GlobchiR = exafs_NeoPars.bestFitPars.globBestVal / (
+                    len(exafs_NeoPars.exafsPars.intervalK) - 3 * exafs_NeoPars.exafsPars.npath + 1)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    STRColors.BOLD + "History Best ChiR: " + STRColors.OKBLUE + str(
+                                                        np.round(GlobchiR, 4)) + STRColors.ENDC, verbose_lvl, 1)
+        STRColors.logger_print_based_on_verbose_lvl(logger, "DiffCounter: " + str(exafs_NeoPars.runPars.diffCounter),
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"Diff %: {(exafs_NeoPars.runPars.diffCounter / exafs_NeoPars.runPars.currGen):.3f}",
+                                                    verbose_lvl, 5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"Mutation Chance: {100 * exafs_NeoPars.mutPars.mutChance:.2f}%",
+                                                    verbose_lvl, 5)
         # if exafs_NeoPars.mutPars.mutOpt == 4:
         #     STRColors.logger_print_based_on_verbose_lvl(logger, "Mutation Percentage" + str(np.round(exafs_NeoPars.self.nmutate_success / self.nmutate, 4)),verbose_lvl,5)
 
-        STRColors.logger_print_based_on_verbose_lvl(logger, "Time: " + str(round(exafs_NeoPars.runPars.currGen_tt, 5)) + "s",verbose_lvl,5)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    "Time: " + str(round(exafs_NeoPars.runPars.currGen_tt, 5)) + "s",
+                                                    verbose_lvl, 5)
 
     @staticmethod
     def run_verbose_end(logger, exafs_NeoPars, verbose_lvl=5):
         """
         Verbose end
         """
 
-        STRColors.logger_print_based_on_verbose_lvl(logger, "-----------Output Stats---------------",verbose_lvl,1)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Total Time(s){STRColors.ENDC}: {round(exafs_NeoPars.runPars.tt, 4)}",verbose_lvl,1)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}File{STRColors.ENDC}: {exafs_NeoPars.neoFilePars.data_path}",verbose_lvl,1)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Path{STRColors.ENDC}: {exafs_NeoPars.exafsPathPars.path_lists}",verbose_lvl,1)
-        STRColors.logger_print_based_on_verbose_lvl(logger, f"{STRColors.BOLD}Final Fittness Score{STRColors.ENDC}: {exafs_NeoPars.bestFitPars.globBestVal:.2f}",verbose_lvl,1)
-        STRColors.logger_print_based_on_verbose_lvl(logger, "-------------------------------------------",verbose_lvl,1)
+        STRColors.logger_print_based_on_verbose_lvl(logger, "-----------Output Stats---------------", verbose_lvl, 1)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Total Time(s){STRColors.ENDC}: {round(exafs_NeoPars.runPars.tt, 4)}",
+                                                    verbose_lvl, 1)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}File{STRColors.ENDC}: {exafs_NeoPars.neoFilePars.data_path}",
+                                                    verbose_lvl, 1)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Path{STRColors.ENDC}: {exafs_NeoPars.exafsPathPars.path_lists}",
+                                                    verbose_lvl, 1)
+        STRColors.logger_print_based_on_verbose_lvl(logger,
+                                                    f"{STRColors.BOLD}Final Fittness Score{STRColors.ENDC}: {exafs_NeoPars.bestFitPars.globBestVal:.2f}",
+                                                    verbose_lvl, 1)
+        STRColors.logger_print_based_on_verbose_lvl(logger, "-------------------------------------------", verbose_lvl,
+                                                    1)
         if exafs_NeoPars.fixedPars.printGraph:
-            # TODO: Reimplment this
+            # TODO: Reimplement this
             pass
             # self.verbose_graph()
 
 
 if __name__ == "__main__":
     # Testing Logger
     # logger = NeoLogger()
```

### Comparing `exafs_neo-2.0.1/exafs_neo.egg-info/PKG-INFO` & `exafs_neo-2.0.2/exafs_neo.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,109 +1,131 @@
 Metadata-Version: 2.1
-Name: exafs-neo
-Version: 2.0.1
+Name: exafs_neo
+Version: 2.0.2
 Summary: exafs_neo AI analysis using GA
 Home-page: https://github.com/laumiulun/EXAFS_Neo
 Download-URL: https://github.com/laumiulun/EXAFS_Neo/tarball/master
 Author: Miu Lun Lau, Jeff Terry, Min Long
 Author-email: andylau@u.boisestate.edu, jterry98@iit.edu, minlong@boisestate.edu
 License: GPLv3
 Keywords: exafs_neo,AI,analysis
+Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: xraylarch
+Requires-Dist: attrs
+Requires-Dist: matplotlib
+Requires-Dist: psutil
 
 # EXAFS Neo
 
-#### Versions: 2.0.0
+#### Versions: 2.0.2
 
-#### Last update: Mar 22, 2021
+#### Last update: Mar 23, 2024
 
 <!-- ![example workflow](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/<WORKFLOW_FILE>/badge.svg) -->
 
-[![Test with Ubuntu, Miniconda](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=unit_tests)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Miniconda](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=unit_tests)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
+[![Test with Ubuntu, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_ubuntu.yml)[![Test with Windows, Mamba](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml/badge.svg?branch=devel)](https://github.com/laumiulun/EXAFS_Neo/actions/workflows/test_windows.yml)
+
 
 EXAFS Neo utilize Genetic algorithm in fitting Extended X-ray absorption fine structure(EXAFS).
 
 ## Prerequisites
 
 It is highly recommend to utilize `anaconda` or `pip` package managers to prevent unforeseen dependency conflicts. EXAFS Neo uses [`larch`](https://xraypy.github.io/xraylarch/) to process the x-ray spectrum.
 
 - Python: => 3.9
 - Numpy: => 1.20
 - Scipy: => 1.6
 - Larch: > 0.9.47
 - Matplotlib: > 3.0
 
-It is highly recommend to create a new environment in `anaconda` to run EXAFS Neo to prevent packages conflicts. For `Windows` operating system, if you encounter a issue requiring "Microsoft C++ 14.0 or greater is needed", please download the tools at the following location [`C++ Tools`](https://visualstudio.microsoft.com/visual-cpp-build-tools/) and make sure to select C++ build tools during installation process.
+It is highly recommend to create a new environment in `anaconda` to run EXAFS Neo to prevent packages conflicts. For `Windows` operating system, if you encounter an issue requiring "Microsoft C++ 14.0 or greater is needed", please download the tools at the following location [`C++ Tools`](https://visualstudio.microsoft.com/visual-cpp-build-tools/) and make sure to select C++ build tools during installation process.
 
 if you are on a Mac (either Intel or M1), you need to make sure that xcode command line tools is install, if not input this command into terminal:
 
         xcode-select --install
 
 ## Dependencies
 
 EXAFS Neo requires the following dependencies to run:
 
         # Create new anaconda environment
         conda create -y --name exafs python=>3.9.10
         conda activate exafs
-        conda install -y "numpy=>1.20" "scipy=>1.6" "matplotlib=>3.0" scikit-learn pandas
-        conda install -y -c conda-forge wxpython pymatgen tomopy pycifrw
+        conda install -y -c conda-forge "numpy>=1.23" "scipy>=1.8" "matplotlib>=3.6" "h5py>=3.5" "wxpython>=4.1" scikit-image scikit-learn pycifrw pandas jupyter plotly pyparsing pytest pytest-cov coverage
+        pip install lmfit peakutils pyepics pyshortcuts termcolor sphinx dill pycifrw xraydb wxmplot wxutils fabio silx imageio charset-normalizer
         pip install xraylarch
 
 ## Installations
 
 To install EXAFS Neo, simply clone the repo:
 
         git clone https://github.com/laumiulun/EXAFS_Neo.git
         cd EXAFS_Neo/
         pip install .
 
 ## Usage
 
-To run a sample test, make sure the environment is set correctly, and select a input file:
+To run the included test suite, use the following command:
+
+        ./run_tests
+
+To run a sample test, make sure the environment is set correctly, and select an input file:
 
          exafs_neo -i test_inputs/test_temp.ini
 
 Alternatively, you can also run EXAFS Neo in a jupyter notebook, please follow the example in the example/jupyter folder
 
-The datafile requires header contain at least either a combination of (k, chi) or (energy, mu). It also requires a minimum of one newline for it to work correctly. An example of the correct header is as follow:
+## GUI
+
+We also have provided a GUI for use in additions to our program, with additional helper script to facilitate post-analysis. To use the GUI:
+
+        exafs_neo_gui
+
+The datafile requires header contain at least either a combination of (k, chi) or (energy, mu). It also requires a minimum of one newline for it to work correctly. An example of the correct header is as follows:
 
         #---------------------------------------------------------------------
         #  k chi chik chik2 chik3 win energy
 
 ## Self adsorption correction
 
-EXAFS also provides a internal option to perform self-adsorption on the sample file using Booth et al correction. This is performed using git submodules:
+EXAFS also provides an internal option to perform self-adsorption on the sample file using Booth et al. correction. This is performed using git submodules:
 
         git submodule update --init --recursive
         cd contrib/sabcor/
         make
 
 ## Update
 
 EXAFS Neo is under active development, to update the code after pulling from the repository:
 
         git pull --rebase
         python setup.py install
 
-## GUI
-
-We also have provided a GUI for use in additions to our program, with additional helper script to facilitate post-analysis. To use the GUI:
 
-        cd gui/
-        python XAFS_GUI.py
 
 ## Video Demonstrations
 
 You can see a list of video demonstrations of the EXAFS Neo package presented, future presentation related to this software will be posted as they are available
 
-<!-- - https://www.youtube.com/playlist?list=PLqZCvArs4yF8IrREQ3AzZJX2N-IRAPEmy [Aug 23,2021] (IIT EXAFS Workshop 2021)
+<!-- - https://www.youtube.com/playlist?list=PLqZCvArs4yF8IrREQ3AzZJX2N-IRAPEmy [Aug 23, 2021] (IIT EXAFS Workshop 2021)
 - https://youtu.be/KwhItvwhapg [Feb 15, 2021] (University of Washington)
 - https://youtu.be/jqISqq_FFR8 [Dec 10, 2020] (Canadian Light Source) -->
 
-- [IIT EXAFS Workshop 2021](https://www.youtube.com/playlist?list=PLqZCvArs4yF8IrREQ3AzZJX2N-IRAPEmy) (Aug 23,2021)
+- [IIT EXAFS Workshop 2021](https://www.youtube.com/playlist?list=PLqZCvArs4yF8IrREQ3AzZJX2N-IRAPEmy) (Aug 23, 2021)
 - [University of Washington](https://youtu.be/KwhItvwhapg) (Feb 15, 2021)
 - [Canadian Light Source](https://youtu.be/jqISqq_FFR8) (Dec 10, 2020)
 
 ## Citation
 
 Jeff Terry, Miu Lun Lau, Jiateng Sun, Chang Xu, Bryan Hendricks, Julia Kise, Mrinalini Lnu, Sanchayni Bagade, Shail Shah, Priyanka Makhijani, Adithya Karantha, Travis Boltz, Max Oellien, Matthew Adas, Shlomo Argamon, Min Long, and Donna Post Guillen, “Analysis of Extended X-ray Absorption Fine Structure (EXAFS) Data Using Artificial Intelligence Techniques,” Applied Surface Science 547, 149059 <https://doi.org/10.1016/j.apsusc.2021.149059> (2021).
+
+    @article{terry2021analysis,
+      title={Analysis of extended X-ray absorption fine structure (EXAFS) data using artificial intelligence techniques},
+      author={Terry, Jeff and Lau, Miu Lun and Sun, Jiateng and Xu, Chang and Hendricks, Bryan and Kise, Julia and Lnu, Mrinalini and Bagade, Sanchayni and Shah, Shail and Makhijani, Priyanka and others},
+      journal={Applied Surface Science},
+      volume={547},
+      pages={149059},
+      year={2021},
+      publisher={Elsevier}
+    }
```

### Comparing `exafs_neo-2.0.1/setup.py` & `exafs_neo-2.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # coding: utf-8
 from __future__ import print_function, unicode_literals
 import sys
 import codecs
 from setuptools import setup, find_packages
 from exafs_neo._version import __version__, __author__, __email__
 
-
 with open('requirements.txt') as f:
     requirements = [l for l in f.read().splitlines() if l]
 
 
 def long_description():
     with codecs.open('README.md', 'rb') as readme:
         if not sys.version_info < (3, 0, 0):
@@ -21,26 +20,28 @@
     version=__version__,
     packages=find_packages(),
     author=__author__,
     author_email=__email__,
     keywords=['exafs_neo', 'AI', 'analysis'],
     description='exafs_neo AI analysis using GA',
     long_description=long_description(),
+    long_description_content_type="text/markdown",
     url='https://github.com/laumiulun/EXAFS_Neo',
     download_url='https://github.com/laumiulun/EXAFS_Neo/tarball/master',
+    package_data={"gui": ["media/*"]},
     include_package_data=True,
     zip_safe=False,
-
     install_requires=[
         'numpy',
         'xraylarch',
         'attrs',
         'matplotlib',
         'psutil'
     ],
     entry_points={
         'console_scripts': [
             'exafs_neo = exafs_neo.input_arg:main',
+            'exafs_neo_gui = exafs_neo.gui.XAFS_GUI:main',
         ]
     },
     license='GPLv3',
 )
```

### Comparing `exafs_neo-2.0.1/tests/test_EXAFS_analysis.py` & `exafs_neo-2.0.2/tests/test_EXAFS_analysis.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,56 +5,35 @@
 import larch
 import os
 import unittest
 import numpy as np
 from pathlib import Path
 
 sys.path.append('gui')
-from gui import EXAFS_Analysis, larch_score
+from exafs_neo.analysis import EXAFS_Analysis, larch_score
 
 
 class TestCase(unittest.TestCase):
     mylarch = larch.Interpreter()
-    params = {}
-    params['base'] = Path(os.getcwd())
-    params['Kmin'] = 2.5
-    params['Kmax'] = 12.5
-    params['kweight'] = 2.0
-    params['deltak'] = 0.05
-    params['rbkg'] = 1.0
-    params['bkgkw'] = 2.0
-    params['bkgkmax'] = 15.0
-    params['front'] = ["cu_test_files/cu_paths/path_75/feff"]
-    params['CSV'] = "cu_test_files/cu_paths/cu_10k.xmu"
-    params['optimize'] = False
-    params['series_index'] = 0
-    params['series'] = False
-    dirs = 'cu_test_files/cu_results/'
+    params = {'base': Path(os.getcwd()), 'Kmin': 2.5, 'Kmax': 12.5, 'kweight': 2.0, 'deltak': 0.05, 'rbkg': 1.0,
+              'bkgkw': 2.0, 'bkgkmax': 15.0, 'front': ["tests/cu_test_files/cu_paths/path_75/feff"],
+              'CSV': "tests/cu_test_files/cu_paths/cu_10k.xmu", 'optimize': False, 'series_index': 0, 'series': False}
+    dirs = 'tests/cu_test_files/cu_results/'
 
     paths = [1, 2, 3, 5, 6, 10, 14, 16, 28, 30, 36, 40, 42]
     larch_score.larch_init(params['CSV'], params)
 
     Test_Result = EXAFS_Analysis.EXAFS_Analysis(paths, dirs, params)
 
-    # def test_construct_full_err(self):
-
-    #     return 0
-    # def test_larch_init(self):
-    #     """
-    #     test larch init
-    #     """
-
-    #     return 0
-
     def test_larch_extract_data_shape(self):
         """
         Test larch extract to have the correct matrix shape
         """
         paths = [1, 2, 3, 5, 6, 10, 14, 16, 28, 30, 36, 40, 42]
-        dirs = 'cu_test_files/cu_results/'
+        dirs = 'tests/cu_test_files/cu_results/'
 
         Test_Result = EXAFS_Analysis.EXAFS_Analysis(paths, dirs, TestCase.params)
 
         TestCase.Test_Result.extract_data(verbose=False)
         result_shape = TestCase.Test_Result.bestFit_mat.shape
         self.assertEqual(result_shape[0], 13)
         self.assertEqual(result_shape[1], 4)
@@ -76,15 +55,14 @@
                                 [0.22, 0.13, 0.008, -0.07],
                                 [0.95, 0.13, 0.006, -0.09],
                                 [0.66, 0.13, 0.001, -0.06],
                                 [0.75, 0.13, 0.001, 0.01],
                                 [0.85, 0.13, 0.004, -0.08]])
 
         self.assertTrue(np.allclose(test_result, real_result))
-        # self.assertTrue((test_result == real_result).all())
 
     def test_chi(self):
         """
         Test larch score data
         """
         TestCase.Test_Result.extract_data(verbose=False)
         TestCase.Test_Result.larch_init()
```

### Comparing `exafs_neo-2.0.1/tests/test_exafs_pars.py` & `exafs_neo-2.0.2/tests/test_exafs_pars.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 import numpy as np
 
 from exafs_neo.neoPars import NeoPars, NeoMutPars
 
 
 class TestEXAFSpars(unittest.TestCase):
-    inputs_pars = {'data_file': '../path_files/Cu/cu_10k.xmu', 'output_file': '',
-                   'feff_file': '../path_files/Cu/path_75/feff', 'kmin': 0.95,
+    inputs_pars = {'data_file': 'tests/cu_test_files/cu_paths/cu_10k.xmu',
+                   'output_file': '',
+                   'feff_file': 'tests/cu_test_files/cu_paths/path_75/feff',
+                   'kmin': 0.95,
                    'kmax': 9.775,
                    'kweight': 3.0, 'pathrange': [1, 2, 3, 4, 5],
                    'deltak': 0.05, 'rbkg': 1.2, 'bkgkw': 1.0, 'bkgkmax': 15.0}
     exafs_NeoPars = NeoPars()
 
     exafs_NeoPars.read_inputs(inputs_pars)
-    print(exafs_NeoPars.exafsPars.npath)
 
     def test_EXAFS_pars(self):
         self.assertEqual(TestEXAFSpars.exafs_NeoPars.exafsPars.kmin, 0.95)
         self.assertEqual(TestEXAFSpars.exafs_NeoPars.exafsPars.kmax, 9.775)
         self.assertEqual(TestEXAFSpars.exafs_NeoPars.exafsPars.dk, 0.05)
         self.assertEqual(TestEXAFSpars.exafs_NeoPars.exafsPars.kweight, 3.0)
         self.assertEqual(TestEXAFSpars.exafs_NeoPars.exafsPars.rbkg, 1.2)
@@ -40,17 +41,17 @@
 
     def test_mutPars(self):
         mutPars = NeoMutPars()
         pass
 
 
 class TestNeoPars(unittest.TestCase):
-    inputs_pars = {'data_file': '../path_files/Cu/cu_10k.xmu',
+    inputs_pars = {'data_file': 'tests/cu_test_files/cu_paths/cu_10k.xmu',
                    'output_file': 'test_output.csv',
-                   'feff_file': '../path_files/Cu/path_75/feff',
+                   'feff_file': 'tests/cu_test_files/cu_paths/path_75/feff',
                    'kmin': 0.95,
                    'kmax': 9.775,
                    'kweight': 3.0,
                    'pathrange': [1, 2, 3, 4, 5],
                    'deltak': 0.05, 'rbkg': 1.2, 'bkgkw': 1.0, 'bkgkmax': 15.0, 'nPops': 150, 'nGen': 200,
                    'mutChance': 0.15}
 
@@ -62,17 +63,17 @@
 
     def test_fixedPars(self):
         self.assertEqual(TestNeoPars.exafs_NeoPars.fixedPars.nPops, 150)
         self.assertEqual(TestNeoPars.exafs_NeoPars.fixedPars.nGen, 200)
         self.assertEqual(TestNeoPars.exafs_NeoPars.fixedPars.selOpt, 0)
 
     def test_filePars(self):
-        self.assertEqual(TestNeoPars.exafs_NeoPars.neoFilePars.data_file, '../path_files/Cu/cu_10k.xmu')
+        # self.assertEqual(TestNeoPars.exafs_NeoPars.neoFilePars.data_file, 'cu_test_files/cu_paths/cu_10k.xmu')
         self.assertEqual(TestNeoPars.exafs_NeoPars.neoFilePars.output_file, 'test_output.csv')
-        self.assertEqual(TestNeoPars.exafs_NeoPars.neoFilePars.feff_file, '../path_files/Cu/path_75/feff')
+        # self.assertEqual(TestNeoPars.exafs_NeoPars.neoFilePars.feff_file, 'cu_test_files/cu_paths/path_75/feff')
 
     def test_mutPars(self):
         self.assertEqual(TestNeoPars.exafs_NeoPars.mutPars.mutOpt, 1)
         self.assertEqual(TestNeoPars.exafs_NeoPars.mutPars.mutChance, 0.15)
         self.assertEqual(TestNeoPars.exafs_NeoPars.mutPars.mutChanceE0, 0.3)
 
     def test_crossPars(self):
```

### Comparing `exafs_neo-2.0.1/tests/test_exafs_pathObj.py` & `exafs_neo-2.0.2/tests/test_exafs_pathObj.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,37 +25,14 @@
 
     def test_getvar_shape(self):
         """Test shape of the get_var method
         """
         var_result = np.array(Test_PathObj.pathObj.get_var())
         self.assertEqual(var_result.shape[0], 3)
 
-    # def test_getS02_value(self):
-    #     """Test the value of s02
-    #     """
-    #     s02 = Test_PathObj.pathObj.s2
-    #     self.assertEqual(s02, Test_PathObj.pathObj.s02)
-
-    # def test_gete0_value(self):
-    #     """Test the value of e0
-    #     """
-    #     e0 = Test_PathObj.pathObj.get_e0()
-    #     self.assertEqual(e0, Test_PathObj.pathObj.e0)
-
-    # def test_getsigma2_value(self):
-    #     """Test the value of sigma2
-    #     """
-    #     sigma2 = Test_PathObj.pathObj.get_sigma2()
-    #     self.assertEqual(sigma2, Test_PathObj.pathObj.sigma2)
-
-    # def test_getdeltaR_value(self):
-    #     """Test the value of deltaR
-    #     """
-    #     deltaR = Test_PathObj.pathObj.get_deltaR()
-    #     self.assertEqual(deltaR, Test_PathObj.pathObj.deltaR)
 
     def test_set_val(self):
         """Test the set method
         """
         pars = Test_PathObj.pathObj.get()
         Test_PathObj.pathObj.set(1, 2, 3)
         self.assertEqual(Test_PathObj.pathObj.s02, 1)
```

### Comparing `exafs_neo-2.0.1/tests/test_exafs_pathrange.py` & `exafs_neo-2.0.2/tests/test_exafs_pathrange.py`

 * *Files identical despite different names*

### Comparing `exafs_neo-2.0.1/tests/test_larchscore.py` & `exafs_neo-2.0.2/tests/test_larchscore.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,38 +3,26 @@
 """
 import larch
 from larch.xafs import autobk, xftf
 
 import os
 import unittest
 from pathlib import Path
-from gui import larch_score
+from exafs_neo.analysis import larch_score
 
 
 class Test_Larchscore(unittest.TestCase):
     # Create a different global interpetor for larch
 
     mylarch = larch.Interpreter()
-    params = {}
-    params['base'] = Path(os.getcwd())
-    params['Kmin'] = 2.5
-    params['Kmax'] = 12.5
-    params['kweight'] = 2.0
-    params['deltak'] = 0.05
-    params['rbkg'] = 1.0
-    params['bkgkw'] = 2.0
-    params['bkgkmax'] = 15.0
-    params['front'] = ["tests/cu_test_files/cu_paths/path_75/feff"]
-    params['CSV'] = "cu_test_files/cu_paths/cu_10k.xmu"
-    params['optimize'] = 'False'
-    params['series_index'] = 0
-    params['series'] = False
-    dirs = 'cu_test_files/cu_results_2/'
+    params = {'base': Path(os.getcwd()), 'Kmin': 2.5, 'Kmax': 12.5, 'kweight': 2.0, 'deltak': 0.05, 'rbkg': 1.0,
+              'bkgkw': 2.0, 'bkgkmax': 15.0, 'front': ["tests/cu_test_files/cu_paths/path_75/feff"],
+              'CSV': "tests/cu_test_files/cu_paths/cu_10k.xmu", 'optimize': 'False', 'series_index': 0, 'series': False}
+    dirs = 'tests/cu_test_files/cu_results_2/'
 
-    print(params['base'])
 
     def test_generate_label_single(self):
         """
         Test Labels with one label
         """
         data = [1]
         result_label = ['s02_1', 'e0', 'sigma_1', 'deltaR_1']
@@ -69,15 +57,14 @@
         result = larch_score.flatten_2d_list(x)
         self.assertEqual(result, [1, 2, 3, 1, 2, 3])
 
     def test_larch_init_params(self):
         """
         Check larch spacing and the resulting output
         """
-
         result = larch_score.larch_init(self.params['CSV'], Test_Larchscore.params)
 
         params = result[2]
 
         self.assertEqual(params['SMALL'], int(self.params['Kmin'] / self.params['deltak']))
         self.assertEqual(params['BIG'], int(self.params['Kmax'] / self.params['deltak']))
 
@@ -85,29 +72,22 @@
         """
         Check Larch Xftf
         """
         # get the exp, which should be g.chi
         result = larch_score.larch_init(self.params['CSV'], Test_Larchscore.params)
         exp = result[0]
 
-        # compared againast manually test
+        # compared against manually test
         file_path = os.path.join(Test_Larchscore.params['base'], Test_Larchscore.params['CSV'])
         g = larch.io.read_ascii(file_path)
 
         autobk(g, rbkg=Test_Larchscore.params['rbkg'],
                kweight=Test_Larchscore.params['bkgkw'],
                kmax=Test_Larchscore.params['bkgkmax'])
         xftf(g.k, g.chi, kmin=Test_Larchscore.params['Kmin'],
              kmax=Test_Larchscore.params['Kmax'],
              dk=4, window='hanning',
              kweight=Test_Larchscore.params['kweight'],
              group=g)
 
         # self.assertTrue(np.allclose(exp, g.chi))
         self.assertTrue((exp == g.chi).all())
-    # def test_latex_table(self):
-    #     """Test Latex table
-    #     """
-
-    #     # larch_score.latex_table()
-    #     return 0
-    # def test_fitness(self):
```

### Comparing `exafs_neo-2.0.1/tests/test_neo_pop.py` & `exafs_neo-2.0.2/tests/test_neo_pop.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 
 from exafs_neo.exafs_pop import NeoPopulations
 from exafs_neo.neoPars import NeoPars
 
 
 class MyTestCase(unittest.TestCase):
 
-    def test_something(self):
-        inputs_pars = {'data_file': '../path_files/Cu/cu_10k.xmu', 'output_file': '',
-                       'feff_file': '../path_files/Cu/path_75/feff', 'kmin': 0.95,
+    def test_neoPars(self):
+        inputs_pars = {'data_file': 'tests/cu_test_files/cu_paths/cu_10k.xmu',
+                       'output_file': '',
+                       'feff_file': 'tests/cu_test_files/cu_paths/path_75/feff',
+                       'kmin': 0.95,
                        'kmax': 9.775,
                        'kweight': 3.0, 'pathrange': [1, 2, 3, 4, 5],
                        'deltak': 0.05, 'rbkg': 1.1, 'bkgkw': 1.0, 'bkgkmax': 15.0}
         exafs_NeoPars = NeoPars()
         exafs_NeoPars.read_inputs(inputs_pars)
         neo_population = NeoPopulations(exafs_NeoPars)
         neo_population.initialize_populations()
         self.assertIsInstance(neo_population[0], tuple)
         # self.assertIsInstance(neo_population[0][0], exafs_test.individual.Individual)
 
 
-# add assertion here
-
-
 if __name__ == '__main__':
     unittest.main()
```

