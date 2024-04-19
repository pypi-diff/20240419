# Comparing `tmp/mvesuvio-0.0.0.dev163.tar.gz` & `tmp/mvesuvio-0.0.0.dev181.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvesuvio-0.0.0.dev163.tar", last modified: Sat Mar 16 02:21:03 2024, max compression
+gzip compressed data, was "mvesuvio-0.0.0.dev181.tar", last modified: Fri Apr 19 08:53:35 2024, max compression
```

## Comparing `mvesuvio-0.0.0.dev163.tar` & `mvesuvio-0.0.0.dev181.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:21:03.669379 mvesuvio-0.0.0.dev163/
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-03-16 02:21:03.669379 mvesuvio-0.0.0.dev163/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:21:03.661378 mvesuvio-0.0.0.dev163/mvesuvio/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-16 02:21:03.000000 mvesuvio-0.0.0.dev163/mvesuvio/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/analysis_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:21:03.665378 mvesuvio-0.0.0.dev163/mvesuvio/config/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/config/Mantid.user.properties
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/config/analysis_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:21:03.665378 mvesuvio-0.0.0.dev163/mvesuvio/config/ip_files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/config/ip_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/config/ip_files/ip2018.par
--rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/config/ip_files/ip2018_2.par
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/config/ip_files/ip2018_3.par
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/config/ip_files/ip2019.par
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/config/vesuvio.user.properties
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:21:03.665378 mvesuvio-0.0.0.dev163/mvesuvio/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/scripts/handle_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:21:03.665378 mvesuvio-0.0.0.dev163/mvesuvio/system_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/system_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/system_tests/analysis_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/system_tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/system_tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/system_tests/test_jackknife.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/system_tests/test_yspace_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/system_tests/test_yspace_fit_GC.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/system_tests/tests_IC.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:21:03.669379 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/ICHelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41027 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/analysis_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22158 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)    20979 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/bootstrap_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/deprecated_mantid_global_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    63650 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/fit_in_yspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     7963 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/procedures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/run_script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:21:03.669379 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/tests/test_analysis_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 02:21:03.669379 mvesuvio-0.0.0.dev163/mvesuvio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-03-16 02:21:03.000000 mvesuvio-0.0.0.dev163/mvesuvio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-16 02:21:03.000000 mvesuvio-0.0.0.dev163/mvesuvio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 02:21:03.000000 mvesuvio-0.0.0.dev163/mvesuvio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-16 02:21:03.000000 mvesuvio-0.0.0.dev163/mvesuvio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-16 02:21:03.000000 mvesuvio-0.0.0.dev163/mvesuvio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-16 02:21:03.000000 mvesuvio-0.0.0.dev163/mvesuvio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-16 02:15:31.000000 mvesuvio-0.0.0.dev163/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 02:21:03.669379 mvesuvio-0.0.0.dev163/setup.cfg
+drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.037948 mvesuvio-0.0.0.dev181/
+-rw-r--r--   0 ljg28444 (1219131)  1219131     6536 2024-04-19 08:53:35.037948 mvesuvio-0.0.0.dev181/PKG-INFO
+-rw-r--r--   0 ljg28444 (1219131)  1219131     5589 2024-04-19 08:51:56.000000 mvesuvio-0.0.0.dev181/README.md
+drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.029948 mvesuvio-0.0.0.dev181/mvesuvio/
+-rw-r--r--   0 ljg28444 (1219131)  1219131     1268 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/__init__.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131       29 2024-04-19 08:53:34.000000 mvesuvio-0.0.0.dev181/mvesuvio/_version.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     1292 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/analysis_runner.py
+drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.029948 mvesuvio-0.0.0.dev181/mvesuvio/config/
+-rw-r--r--   0 ljg28444 (1219131)  1219131       77 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/Mantid.user.properties
+-rw-r--r--   0 ljg28444 (1219131)  1219131        0 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/__init__.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     5026 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/analysis_inputs.py
+drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.029948 mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/
+-rw-r--r--   0 ljg28444 (1219131)  1219131        0 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/__init__.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     7027 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2018.par
+-rw-r--r--   0 ljg28444 (1219131)  1219131     7218 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2018_2.par
+-rw-r--r--   0 ljg28444 (1219131)  1219131     7079 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2018_3.par
+-rw-r--r--   0 ljg28444 (1219131)  1219131     4291 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2019.par
+-rw-r--r--   0 ljg28444 (1219131)  1219131       87 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/vesuvio.user.properties
+drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.029948 mvesuvio-0.0.0.dev181/mvesuvio/scripts/
+-rw-r--r--   0 ljg28444 (1219131)  1219131     2758 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/scripts/__init__.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     3907 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/scripts/handle_config.py
+drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.033948 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/
+-rw-r--r--   0 ljg28444 (1219131)  1219131        0 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/__init__.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     5900 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_analysis.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     4173 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_bootstrap.py
+drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.033948 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_config/
+-rw-r--r--   0 ljg28444 (1219131)  1219131        0 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_config/__init__.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     3836 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_config/expr_for_tests.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     2225 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_jackknife.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     5664 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_yspace_fit.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     5676 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_yspace_fit_GC.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     4723 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/tests_IC.py
+drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.037948 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/
+-rw-r--r--   0 ljg28444 (1219131)  1219131    10860 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/ICHelpers.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131        0 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/__init__.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131    41027 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/analysis_functions.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131    22158 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/bootstrap.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131    20979 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/bootstrap_analysis.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     6506 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/deprecated_mantid_global_fit.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131    63650 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/fit_in_yspace.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     7963 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/procedures.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131     4573 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/run_script.py
+drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.037948 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/tests/
+-rw-r--r--   0 ljg28444 (1219131)  1219131        0 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/tests/__init__.py
+-rw-r--r--   0 ljg28444 (1219131)  1219131      746 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/tests/test_analysis_functions.py
+drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.037948 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/
+-rw-r--r--   0 ljg28444 (1219131)  1219131     6536 2024-04-19 08:53:35.000000 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/PKG-INFO
+-rw-r--r--   0 ljg28444 (1219131)  1219131     1544 2024-04-19 08:53:35.000000 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/SOURCES.txt
+-rw-r--r--   0 ljg28444 (1219131)  1219131        1 2024-04-19 08:53:35.000000 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/dependency_links.txt
+-rw-r--r--   0 ljg28444 (1219131)  1219131       51 2024-04-19 08:53:35.000000 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/entry_points.txt
+-rw-r--r--   0 ljg28444 (1219131)  1219131       81 2024-04-19 08:53:35.000000 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/requires.txt
+-rw-r--r--   0 ljg28444 (1219131)  1219131        9 2024-04-19 08:53:35.000000 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/top_level.txt
+-rw-r--r--   0 ljg28444 (1219131)  1219131     1921 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/pyproject.toml
+-rw-r--r--   0 ljg28444 (1219131)  1219131       38 2024-04-19 08:53:35.037948 mvesuvio-0.0.0.dev181/setup.cfg
```

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/config/analysis_inputs.py` & `mvesuvio-0.0.0.dev181/mvesuvio/config/analysis_inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     normVoigt = False
 
 
 class YSpaceFitInitialConditions:
     showPlots = True
     symmetrisationFlag = True
     rebinParametersForYSpaceFit = "-25, 0.5, 25"  # Needs to be symetric
-    fitModel = "Gaussian3D"  # Options: 'SINGLE_GAUSSIAN', 'GC_C4', 'GC_C6', 'GC_C4_C6', 'DOUBLE_WELL', 'ANSIO_GAUSSIAN', 'Gaussian3D'
+    fitModel = "SINGLE_GAUSSIAN"  # Options: 'SINGLE_GAUSSIAN', 'GC_C4', 'GC_C6', 'GC_C4_C6', 'DOUBLE_WELL', 'ANSIO_GAUSSIAN', 'Gaussian3D'
     runMinos = True
     globalFit = True  # Performs global fit with Minuit by default
     nGlobalFitGroups = 4  # Number or string "ALL"
     maskTypeProcedure = "NAN"  # Options: 'NCP', 'NAN', None
 
 
 class UserScriptControls:
@@ -156,7 +156,18 @@
 
     # Choose on which ws to perform the fit in y space
     fitInYSpace = "FORWARD"  # Options: None, "BACKWARD", "FORWARD", "JOINT"
 
 
 class BootstrapInitialConditions:
     runBootstrap = False
+
+
+####################
+### RUN ANALYSIS ###
+####################
+
+if (__name__ == "__main__") or (__name__ == "mantidqt.widgets.codeeditor.execution"):
+    import mvesuvio
+    from pathlib import Path
+    mvesuvio.set_config(inputs_file=Path(__file__))
+    mvesuvio.run()
```

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/config/ip_files/ip2018.par` & `mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2018.par`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/config/ip_files/ip2018_2.par` & `mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2018_2.par`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/config/ip_files/ip2018_3.par` & `mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2018_3.par`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/config/ip_files/ip2019.par` & `mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2019.par`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/scripts/__init__.py` & `mvesuvio-0.0.0.dev181/mvesuvio/scripts/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,90 +11,79 @@
         __setup_config(args)
 
     if args.command == "run":
         if not handle_config.config_set():
             __setup_config(None)
         __run_analysis(args.yes)
 
+
 def __setup_and_parse_args():
     parser = __set_up_parser()
     args = parser.parse_args()
     return args
 
+
 def __set_up_parser():
     parser = argparse.ArgumentParser(
         description="Package to analyse Vesuvio instrument data"
     )
     subparsers = parser.add_subparsers(dest="command", required=True)
     config_parser = subparsers.add_parser("config", help="set mvesuvio configuration")
     config_parser.add_argument(
-        "--set-cache", "-c", help="set the cache directory", default="", type=str
+        "--set-inputs", "-i", help="set the inputs python file", default="", type=str
     )
     config_parser.add_argument(
         "--set-ipfolder",
         "-p",
         help="set the intrument parameters directory",
         default="",
         type=str,
     )
-    config_parser.add_argument(
-        "--set-experiment",
-        "-e",
-        help="set the current experiment",
-        default="",
-        type=str,
-    )
 
     run_parser = subparsers.add_parser("run", help="run mvesuvio analysis")
     run_parser.add_argument(
         "--yes", "-y", help="Say yes to all input prompts", action="store_true"
     )
     return parser
 
 
 def __setup_config(args):
     config_dir = handle_config.VESUVIO_CONFIG_PATH
     handle_config.setup_config_dir(config_dir)
     ipfolder_dir = handle_config.VESUVIO_IPFOLDER_PATH
+    inputs = handle_config.VESUVIO_INPUTS_PATH
 
     if handle_config.config_set():
-        cache_dir = (
-            handle_config.read_config_var("caching.location")
-            if not args or not args.set_cache
-            else args.set_cache
-        )
-        experiment = (
-            handle_config.read_config_var("caching.experiment")
-            if not args or not args.set_experiment
-            else args.set_experiment
+        inputs = (
+            handle_config.read_config_var("caching.inputs")
+            if not args or not args.set_inputs
+            else args.set_inputs
         )
         ipfolder_dir = (
             handle_config.read_config_var("caching.ipfolder")
             if not args or not args.set_ipfolder
             else args.set_ipfolder
         )
     else:
-        cache_dir = config_dir if not args or not args.set_cache else args.set_cache
-        experiment = (
-            "default" if not args or not args.set_experiment else args.set_experiment
+        inputs = (
+            inputs if not args or not args.set_inputs else args.set_inputs
         )
         ipfolder_dir = (
             ipfolder_dir if not args or not args.set_ipfolder else args.set_ipfolder
         )
 
         handle_config.setup_default_ipfile_dir()
+        handle_config.setup_default_inputs()
 
     handle_config.set_config_vars(
         {
-            "caching.location": cache_dir,
-            "caching.experiment": experiment,
+            "caching.inputs": inputs,
             "caching.ipfolder": ipfolder_dir,
         }
     )
-    handle_config.setup_expr_dir(cache_dir, experiment)
     handle_config.check_dir_exists("IP folder", ipfolder_dir)
 
 
 def __run_analysis(yes_to_all):
     environ["MANTIDPROPERTIES"] = path.join(
         handle_config.VESUVIO_CONFIG_PATH, "Mantid.user.properties"
     )
```

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/scripts/handle_config.py` & `mvesuvio-0.0.0.dev181/mvesuvio/scripts/handle_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         config_file = "vesuvio.user.properties"
     return config_path, config_file
 
 
 ### PATH CONSTANTS ###
 VESUVIO_CONFIG_PATH, VESUVIO_CONFIG_FILE = __parse_config_env_var()
 VESUVIO_INPUTS_FILE = "analysis_inputs.py"
+VESUVIO_INPUTS_PATH = os.path.join(VESUVIO_CONFIG_PATH, VESUVIO_INPUTS_FILE)
 VESUVIO_PACKAGE_PATH = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 MANTID_CONFIG_FILE = "Mantid.user.properties"
 VESUVIO_IPFOLDER_PATH = os.path.join(VESUVIO_CONFIG_PATH, "ip_files")
 ######################
 
 
 def __read_config(config_file_path, throw_on_not_found=True):
@@ -66,34 +67,38 @@
             result = line.split("=", 2)[1].strip("\n")
             break
     if not result and throw_on_not_found:
         raise ValueError(f"{var} was not found in the vesuvio config")
     return result
 
 
+def get_script_name():
+    filename = os.path.basename(read_config_var("caching.inputs"))
+    scriptName = filename.removesuffix(".py")
+    return scriptName
+
+
 def setup_config_dir(config_dir):
     success = __mk_dir("config", config_dir)
     if success:
         copyfile(
             os.path.join(VESUVIO_PACKAGE_PATH, "config", VESUVIO_CONFIG_FILE),
             os.path.join(config_dir, VESUVIO_CONFIG_FILE),
         )
         copyfile(
             os.path.join(VESUVIO_PACKAGE_PATH, "config", MANTID_CONFIG_FILE),
             os.path.join(config_dir, MANTID_CONFIG_FILE),
         )
 
 
-def setup_expr_dir(cache_dir, experiment):
-    expr_path = os.path.join(cache_dir, "experiments", experiment)
-    success = __mk_dir("experiment", expr_path)
-    if success:
+def setup_default_inputs():
+    if not os.path.isfile(VESUVIO_INPUTS_PATH):
         copyfile(
             os.path.join(VESUVIO_PACKAGE_PATH, "config", VESUVIO_INPUTS_FILE),
-            input_file_path(cache_dir, experiment),
+            os.path.join(VESUVIO_INPUTS_PATH),
         )
 
 
 def setup_default_ipfile_dir():
     if not os.path.isdir(VESUVIO_IPFOLDER_PATH):
         copytree(
             os.path.join(VESUVIO_PACKAGE_PATH, "config", "ip_files"),
@@ -110,22 +115,18 @@
             success = True
         except:
             print(f"Unable to make {type} directory at location: {path}")
     return success
 
 
 def config_set():
-    if read_config_var("caching.location", False):
+    if read_config_var("caching.inputs", False):
         return True
     else:
         return False
 
 
-def input_file_path(cache_dir, experiment):
-    return os.path.join(cache_dir, "experiments", experiment, VESUVIO_INPUTS_FILE)
-
-
 def check_dir_exists(type, path):
     if not os.path.isdir(path):
         print(f"Directory of {type} could not be found at location: {path}")
         return False
     return True
```

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/system_tests/analysis_inputs.py` & `mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_config/expr_for_tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,15 +103,22 @@
     tofBinning = "110,1,430"  # Binning of ToF spectra
     maskTOFRange = None
     runHistData = True
     normVoigt = False
 
 
 class YSpaceFitInitialConditions:
-    anything = True
+    showPlots = False
+    symmetrisationFlag = True
+    rebinParametersForYSpaceFit = "-20, 0.5, 20"  # Needs to be symetric
+    fitModel = "SINGLE_GAUSSIAN"
+    runMinos = True
+    globalFit = None
+    nGlobalFitGroups = 4
+    maskTypeProcedure = None
 
 
 class UserScriptControls:
     runRoutine = True
     procedure = "FORWARD"  # Options: None, "BACKWARD", "FORWARD", "JOINT"
     fitInYSpace = None  # Options: None, "BACKWARD", "FORWARD", "JOINT"
```

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/system_tests/test_analysis.py` & `mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from mvesuvio.vesuvio_analysis.run_script import runScript
 import unittest
 import numpy as np
 import numpy.testing as nptest
 from pathlib import Path
 from mvesuvio.scripts import handle_config
-from mvesuvio.system_tests.analysis_inputs import (
+from mvesuvio.system_tests.test_config.expr_for_tests import (
     LoadVesuvioBackParameters,
     LoadVesuvioFrontParameters,
     BackwardInitialConditions,
     ForwardInitialConditions,
     YSpaceFitInitialConditions,
     BootstrapInitialConditions,
     UserScriptControls,
 )
-
+import mvesuvio
+mvesuvio.set_config(
+    ip_folder=str(Path(handle_config.VESUVIO_PACKAGE_PATH).joinpath("config", "ip_files")),
+    inputs_file=str(Path(handle_config.VESUVIO_PACKAGE_PATH).joinpath("system_tests", "test_config", "expr_for_tests.py"))
+)
 
 ipFilesPath = Path(handle_config.read_config_var("caching.ipfolder"))
 
 
 class AnalysisRunner:
     _benchmarkResults = None
     _currentResults = None
@@ -34,15 +38,14 @@
             cls._run()
         return AnalysisRunner._currentResults
 
     @classmethod
     def _run(cls):
         scattRes, yfitRes = runScript(
             UserScriptControls(),
-            "test_expr",
             LoadVesuvioBackParameters(ipFilesPath),
             LoadVesuvioFrontParameters(ipFilesPath),
             BackwardInitialConditions(ipFilesPath),
             ForwardInitialConditions(ipFilesPath),
             YSpaceFitInitialConditions(),
             BootstrapInitialConditions(),
             True,
```

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/system_tests/test_bootstrap.py` & `mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+
+# This file needs updating once the bootstrap functunality is properly
+# implemented in the mvesuvio package
+
 from mvesuvio.vesuvio_analysis.run_script import runScript
 import unittest
 import numpy as np
 import numpy.testing as nptest
 from pathlib import Path
 from mvesuvio.system_tests.tests_IC import (
-    scriptName,
     wsBackIC,
     wsFrontIC,
     bckwdIC,
     fwdIC,
     yFitIC,
 )
 
-
 class BootstrapInitialConditions:
     runBootstrap = True
 
     procedure = "JOINT"
     fitInYSpace = "FORWARD"
 
     bootstrapType = "BOOT_RESIDUALS"
@@ -41,15 +43,15 @@
         userCtr = UserScriptControls
 
         # Change yFItIC to default settings, running tests for yfit before hand changes this
         yFitIC.fitModel = "SINGLE_GAUSSIAN"
         yFitIC.symmetrisationFlag = True
 
         bootRes, noneRes = runScript(
-            userCtr, scriptName, wsBackIC, wsFrontIC, bckwdIC, fwdIC, yFitIC, bootIC, True
+            userCtr, wsBackIC, wsFrontIC, bckwdIC, fwdIC, yFitIC, bootIC, True
         )
 
         # TODO: Figure out why doing the two tests simultaneously fails the testing
         # Probably because running bootstrap alters the initial conditions of forward scattering
         # Test Joint procedure
 
         cls._bootBackSamples = bootRes["bckwdScat"].bootSamples
```

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/system_tests/test_jackknife.py` & `mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_jackknife.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+
+# This file needs updating once the bootstrap functunality is properly
+# implemented in the mvesuvio package
+
 from mvesuvio.vesuvio_analysis.run_script import runScript
 import unittest
 import numpy as np
 import numpy.testing as nptest
 from pathlib import Path
 from mvesuvio.system_tests.tests_IC import (
-    scriptName,
     wsBackIC,
     wsFrontIC,
     bckwdIC,
     fwdIC,
     yFitIC,
 )
 
@@ -38,15 +41,15 @@
     def _run_analysis(cls):
         np.random.seed(3)  # Set seed so that tests match everytime
 
         bootIC = BootstrapInitialConditions
         userCtr = UserScriptControls
 
         bootRes, noneRes = runScript(
-            userCtr, scriptName, wsBackIC, wsFrontIC, bckwdIC, fwdIC, yFitIC, bootIC, True
+            userCtr, wsBackIC, wsFrontIC, bckwdIC, fwdIC, yFitIC, bootIC, True
         )
 
         cls._jackBackSamples = bootRes["bckwdScat"].bootSamples
         cls._jackFrontSamples = bootRes["fwdScat"].bootSamples
 
         # jackJointResults = bootRes
```

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/system_tests/tests_IC.py` & `mvesuvio-0.0.0.dev181/mvesuvio/system_tests/tests_IC.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/ICHelpers.py` & `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/ICHelpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from mantid.simpleapi import Load, LoadVesuvio, SaveNexus, DeleteWorkspace
 from pathlib import Path
 from mvesuvio.scripts import handle_config
 from mantid.kernel import logger
 import ntpath
 
-experimentsPath = (
-    Path(handle_config.read_config_var("caching.location")) / "experiments"
-)
 
+def _get_expr_path():
+    inputsPath = Path(handle_config.read_config_var("caching.inputs"))
+    scriptName = handle_config.get_script_name()
+    experimentPath = inputsPath.parent / scriptName
+    return experimentPath
 
-def completeICFromInputs(IC, scriptName, wsIC):
+
+def completeICFromInputs(IC, wsIC):
     """Assigns new methods to the initial conditions class from the inputs of that class"""
+    scriptName = handle_config.get_script_name()
 
     assert (
         IC.lastSpec > IC.firstSpec
     ), "Last spectrum needs to be bigger than first spectrum"
     assert ((IC.lastSpec < 135) & (IC.firstSpec < 135)) | (
         (IC.lastSpec >= 135) & (IC.firstSpec >= 135)
     ), "First and last spec need to be both in Back or Front scattering."
@@ -45,35 +49,30 @@
     # When attribute InstrParsPath is not present, set it equal to path from wsIC
     try:
         IC.InstrParsPath  # If present, leave it unaltered
     except AttributeError:
         IC.InstrParsPath = wsIC.ipfile
 
     # Sort out input and output paths
-    rawPath, emptyPath = setInputWSForSample(wsIC, scriptName)
+    rawPath, emptyPath = setInputWSForSample(wsIC)
 
     IC.userWsRawPath = rawPath
     IC.userWsEmptyPath = emptyPath
 
-    setOutputDirsForSample(IC, scriptName)
+    setOutputDirsForSample(IC)
 
     # Do not run bootstrap sample, by default
     IC.runningSampleWS = False
 
     # Store script name
     IC.scriptName = scriptName
 
     # Default not running preliminary procedure to estimate HToMass0Ratio
     IC.runningPreliminary = False
 
-    # Set directories for figures
-    figSavePath = experimentsPath / scriptName / "figures"
-    figSavePath.mkdir(exist_ok=True)
-    IC.figSavePath = figSavePath
-
     # Create default of not running original version with histogram data
     try:
         IC.runHistData
     except AttributeError:
         IC.runHistData = False
 
     # Norm voigt except when comparing with tests
@@ -81,22 +80,25 @@
         IC.normVoigt
     except AttributeError:
         IC.normVoigt = True
 
     return
 
 
-def setInputWSForSample(wsIC, sampleName):
-    inputWSPath = experimentsPath / sampleName / "input_ws"
+def setInputWSForSample(wsIC):
+    experimentPath = _get_expr_path()
+    scriptName = handle_config.get_script_name()
+
+    inputWSPath = experimentPath / "input_ws"
     inputWSPath.mkdir(parents=True, exist_ok=True)
 
     runningMode = getRunningMode(wsIC)
 
-    rawWSName = sampleName + "_" + "raw" + "_" + runningMode + ".nxs"
-    emptyWSName = sampleName + "_" + "empty" + "_" + runningMode + ".nxs"
+    rawWSName = scriptName + "_" + "raw" + "_" + runningMode + ".nxs"
+    emptyWSName = scriptName + "_" + "empty" + "_" + runningMode + ".nxs"
 
     rawPath = inputWSPath / rawWSName
     emptyPath = inputWSPath / emptyWSName
 
     if not wsHistoryMatchesInputs(wsIC.runs, wsIC.mode, wsIC.ipfile, rawPath):
         saveWSFromLoadVesuvio(wsIC.runs, wsIC.mode, wsIC.ipfile, rawPath)
 
@@ -114,16 +116,17 @@
     else:
         raise ValueError(
             f"Input class for loading workspace not valid: {wsIC.__class__.__name__}"
         )
     return runningMode
 
 
-def setOutputDirsForSample(IC, sampleName):
-    outputPath = experimentsPath / sampleName / "output_files"
+def setOutputDirsForSample(IC):
+    experimentPath = _get_expr_path()
+    outputPath = experimentPath / "output_files"
     outputPath.mkdir(parents=True, exist_ok=True)
 
     # Build Filename based on ic
     corr = ""
     if IC.GammaCorrectionFlag & (IC.noOfMSIterations > 0):
         corr += "_GC"
     if IC.MSCorrectionFlag & (IC.noOfMSIterations > 0):
@@ -132,14 +135,19 @@
     fileName = (
         f"spec_{IC.firstSpec}-{IC.lastSpec}_iter_{IC.noOfMSIterations}{corr}" + ".npz"
     )
     fileNameYSpace = fileName + "_ySpaceFit" + ".npz"
 
     IC.resultsSavePath = outputPath / fileName
     IC.ySpaceFitSavePath = outputPath / fileNameYSpace
+
+    # Set directories for figures
+    figSavePath = experimentPath / "figures"
+    figSavePath.mkdir(exist_ok=True)
+    IC.figSavePath = figSavePath
     return
 
 
 def wsHistoryMatchesInputs(runs, mode, ipfile, localPath):
     if not (localPath.is_file()):
         logger.notice("Cached workspace not found")
         return False
@@ -204,26 +212,28 @@
 
     setBootstrapDirs(bckwdIC, fwdIC, bootIC, yFitIC)
     return
 
 
 def setBootstrapDirs(bckwdIC, fwdIC, bootIC, yFitIC):
     """Form bootstrap output data paths"""
+    experimentPath = _get_expr_path()
+    scriptName = handle_config.get_script_name()
 
     # Select script name and experiments path
     sampleName = bckwdIC.scriptName  # Name of sample currently running
 
     # Used to store running times required to estimate Bootstrap total run time.
-    bootIC.runTimesPath = experimentsPath / sampleName / "running_times.txt"
+    bootIC.runTimesPath = experimentPath / "running_times.txt"
 
     # Make bootstrap and jackknife data directories
     if bootIC.bootstrapType == "JACKKNIFE":
-        bootPath = experimentsPath / sampleName / "jackknife_data"
+        bootPath = experimentPath / "jackknife_data"
     else:
-        bootPath = experimentsPath / sampleName / "bootstrap_data"
+        bootPath = experimentPath / "bootstrap_data"
     bootPath.mkdir(exist_ok=True)
 
     # Folders for skipped and unskipped MS
     if bootIC.skipMSIterations:
         dataPath = bootPath / "skip_MS_corrections"
     else:
         dataPath = bootPath / "with_MS_corrections"
@@ -313,20 +323,21 @@
 
 def noOfHistsFromTOFBinning(IC):
     # Convert first to float and then to int because of decimal points
     start, spacing, end = [int(float(s)) for s in IC.tofBinning.split(",")]
     return int((end - start) / spacing) - 1  # To account for last column being ignored
 
 
-def buildFinalWSName(scriptName: str, procedure: str, IC):
+def buildFinalWSName(procedure: str, IC):
+    scriptName = handle_config.get_script_name()
     # Format of corrected ws from last iteration
     name = scriptName + "_" + procedure + "_" + str(IC.noOfMSIterations)
     return name
 
 
-def completeYFitIC(yFitIC, sampleName):
+def completeYFitIC(yFitIC):
+    experimentPath = _get_expr_path()
     # Set directories for figures
-
-    figSavePath = experimentsPath / sampleName / "figures"
+    figSavePath = experimentPath / "figures"
     figSavePath.mkdir(exist_ok=True)
     yFitIC.figSavePath = figSavePath
     return
```

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/analysis_functions.py` & `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/bootstrap.py` & `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/bootstrap.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/bootstrap_analysis.py` & `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/bootstrap_analysis.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/deprecated_mantid_global_fit.py` & `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/deprecated_mantid_global_fit.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/fit_in_yspace.py` & `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/fit_in_yspace.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/procedures.py` & `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/procedures.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/run_script.py` & `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/run_script.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,28 +14,27 @@
     isHPresent,
 )
 from mantid.api import mtd
 
 
 def runScript(
     userCtr,
-    scriptName,
     wsBackIC,
     wsFrontIC,
     bckwdIC,
     fwdIC,
     yFitIC,
     bootIC,
     yes_to_all=False,
 ):
     # Set extra attributes from user attributes
-    completeICFromInputs(fwdIC, scriptName, wsFrontIC)
-    completeICFromInputs(bckwdIC, scriptName, wsBackIC)
+    completeICFromInputs(fwdIC, wsFrontIC)
+    completeICFromInputs(bckwdIC, wsBackIC)
     completeBootIC(bootIC, bckwdIC, fwdIC, yFitIC)
-    completeYFitIC(yFitIC, scriptName)
+    completeYFitIC(yFitIC)
 
     checkInputs(userCtr)
     checkInputs(bootIC)
     assert not (
         userCtr.runRoutine & bootIC.runBootstrap
     ), "Main routine and bootstrap both set to run!"
 
@@ -69,15 +68,15 @@
         return res
 
     # Names of workspaces to be fitted in y space
     wsNames = []
     ICs = []
     for mode, IC in zip(["BACKWARD", "FORWARD"], [bckwdIC, fwdIC]):
         if (userCtr.fitInYSpace == mode) | (userCtr.fitInYSpace == "JOINT"):
-            wsNames.append(buildFinalWSName(scriptName, mode, IC))
+            wsNames.append(buildFinalWSName(mode, IC))
             ICs.append(IC)
 
     # If bootstrap is not None, run bootstrap procedure and finish
     if bootIC.runBootstrap:
         assert (
             (bootIC.procedure == "FORWARD")
             | (bootIC.procedure == "BACKWARD")
```

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio/vesuvio_analysis/tests/test_analysis_functions.py` & `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/tests/test_analysis_functions.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev163/mvesuvio.egg-info/SOURCES.txt` & `mvesuvio-0.0.0.dev181/mvesuvio.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 mvesuvio/config/ip_files/ip2018.par
 mvesuvio/config/ip_files/ip2018_2.par
 mvesuvio/config/ip_files/ip2018_3.par
 mvesuvio/config/ip_files/ip2019.par
 mvesuvio/scripts/__init__.py
 mvesuvio/scripts/handle_config.py
 mvesuvio/system_tests/__init__.py
-mvesuvio/system_tests/analysis_inputs.py
 mvesuvio/system_tests/test_analysis.py
 mvesuvio/system_tests/test_bootstrap.py
 mvesuvio/system_tests/test_jackknife.py
 mvesuvio/system_tests/test_yspace_fit.py
 mvesuvio/system_tests/test_yspace_fit_GC.py
 mvesuvio/system_tests/tests_IC.py
+mvesuvio/system_tests/test_config/__init__.py
+mvesuvio/system_tests/test_config/expr_for_tests.py
 mvesuvio/vesuvio_analysis/ICHelpers.py
 mvesuvio/vesuvio_analysis/__init__.py
 mvesuvio/vesuvio_analysis/analysis_functions.py
 mvesuvio/vesuvio_analysis/bootstrap.py
 mvesuvio/vesuvio_analysis/bootstrap_analysis.py
 mvesuvio/vesuvio_analysis/deprecated_mantid_global_fit.py
 mvesuvio/vesuvio_analysis/fit_in_yspace.py
```

### Comparing `mvesuvio-0.0.0.dev163/pyproject.toml` & `mvesuvio-0.0.0.dev181/pyproject.toml`

 * *Files identical despite different names*

