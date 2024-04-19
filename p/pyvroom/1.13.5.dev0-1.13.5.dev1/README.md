# Comparing `tmp/pyvroom-1.13.5.dev0.tar.gz` & `tmp/pyvroom-1.13.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvroom-1.13.5.dev0.tar", last modified: Thu Apr 11 11:41:30 2024, max compression
+gzip compressed data, was "pyvroom-1.13.5.dev1.tar", last modified: Fri Apr 19 14:19:55 2024, max compression
```

## Comparing `pyvroom-1.13.5.dev0.tar` & `pyvroom-1.13.5.dev1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.312467 pyvroom-1.13.5.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.300467 pyvroom-1.13.5.dev0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.304467 pyvroom-1.13.5.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/.github/workflows/main_push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-11 11:41:30.312467 pyvroom-1.13.5.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/build-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/conanfile.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-11 11:41:30.312467 pyvroom-1.13.5.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.304467 pyvroom-1.13.5.dev0/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/_vroom.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.308467 pyvroom-1.13.5.dev0/src/bind/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/_main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/amount.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/break.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/enums.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/exception.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.308467 pyvroom-1.13.5.dev0/src/bind/generic/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/generic/matrix.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.308467 pyvroom-1.13.5.dev0/src/bind/input/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/input/input.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/input/vehicle_step.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/job.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/location.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.308467 pyvroom-1.13.5.dev0/src/bind/solution/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/solution/route.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/solution/solution.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/solution/step.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/solution/summary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/time_window.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/bind/vehicle.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.312467 pyvroom-1.13.5.dev0/src/pyvroom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-11 11:41:30.000000 pyvroom-1.13.5.dev0/src/pyvroom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-11 11:41:30.000000 pyvroom-1.13.5.dev0/src/pyvroom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:41:30.000000 pyvroom-1.13.5.dev0/src/pyvroom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-11 11:41:30.000000 pyvroom-1.13.5.dev0/src/pyvroom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 11:41:30.000000 pyvroom-1.13.5.dev0/src/pyvroom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 11:41:30.000000 pyvroom-1.13.5.dev0/src/pyvroom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 11:41:30.000000 pyvroom-1.13.5.dev0/src/pyvroom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.308467 pyvroom-1.13.5.dev0/src/vroom/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/break_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.312467 pyvroom-1.13.5.dev0/src/vroom/input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/input/forced_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/input/input.py
--rw-r--r--   0 runner    (1001) docker     (127)    16576 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/input/vehicle_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/location.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.312467 pyvroom-1.13.5.dev0/src/vroom/solution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/solution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/solution/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/time_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/src/vroom/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.312467 pyvroom-1.13.5.dev0/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 11:41:30.312467 pyvroom-1.13.5.dev0/test/input/
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/test/input/test_vehicle_step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/test/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/test/test_break.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/test/test_file_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/test/test_libvroom_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/test/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/test/test_time_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-11 11:41:25.000000 pyvroom-1.13.5.dev0/test/test_vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.052484 pyvroom-1.13.5.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.040484 pyvroom-1.13.5.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.044484 pyvroom-1.13.5.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/.github/workflows/main_push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-19 14:19:55.052484 pyvroom-1.13.5.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/build-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/conanfile.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 14:19:55.052484 pyvroom-1.13.5.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.044484 pyvroom-1.13.5.dev1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/_vroom.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.044484 pyvroom-1.13.5.dev1/src/bind/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/_main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/amount.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/break.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/enums.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/exception.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.044484 pyvroom-1.13.5.dev1/src/bind/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/generic/matrix.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.044484 pyvroom-1.13.5.dev1/src/bind/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/input/input.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/input/vehicle_step.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/job.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/location.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.044484 pyvroom-1.13.5.dev1/src/bind/solution/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/solution/route.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/solution/solution.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/solution/step.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/solution/summary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/time_window.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/bind/vehicle.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.052484 pyvroom-1.13.5.dev1/src/pyvroom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-19 14:19:55.000000 pyvroom-1.13.5.dev1/src/pyvroom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-19 14:19:55.000000 pyvroom-1.13.5.dev1/src/pyvroom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:19:55.000000 pyvroom-1.13.5.dev1/src/pyvroom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 14:19:55.000000 pyvroom-1.13.5.dev1/src/pyvroom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:19:54.000000 pyvroom-1.13.5.dev1/src/pyvroom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 14:19:55.000000 pyvroom-1.13.5.dev1/src/pyvroom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 14:19:55.000000 pyvroom-1.13.5.dev1/src/pyvroom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.048484 pyvroom-1.13.5.dev1/src/vroom/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/break_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.048484 pyvroom-1.13.5.dev1/src/vroom/input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/input/forced_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/input/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16576 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/input/vehicle_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/location.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.048484 pyvroom-1.13.5.dev1/src/vroom/solution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/solution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/solution/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/time_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/src/vroom/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.052484 pyvroom-1.13.5.dev1/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:55.052484 pyvroom-1.13.5.dev1/test/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/test/input/test_vehicle_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/test/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/test/test_break.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/test/test_file_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/test/test_libvroom_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/test/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/test/test_time_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-19 14:19:49.000000 pyvroom-1.13.5.dev1/test/test_vehicle.py
```

### Comparing `pyvroom-1.13.5.dev0/.github/workflows/main_push.yml` & `pyvroom-1.13.5.dev1/.github/workflows/main_push.yml`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/.github/workflows/pull_request.yml` & `pyvroom-1.13.5.dev1/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/.github/workflows/release.yml` & `pyvroom-1.13.5.dev1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/.gitignore` & `pyvroom-1.13.5.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/LICENSE` & `pyvroom-1.13.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/Makefile` & `pyvroom-1.13.5.dev1/Makefile`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/PKG-INFO` & `pyvroom-1.13.5.dev1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pyvroom
-Version: 1.13.5.dev0
-Summary: Vehicle routing open-source optimization machine (VROOM)
-Author: Jonathan Feinberg
-Author-email: jonathf@gmail.com
-License: BSD 2-Clause License
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: pandas
-
 Python Vehicle Routing Open-source Optimization Machine
 =======================================================
 
 |gh_action| |codecov| |pypi|
 
 .. |gh_action| image:: https://img.shields.io/github/checks-status/VROOM-Project/pyvroom/main
     :target: https://github.com/VROOM-Project/pyvroom/actions
@@ -107,15 +92,15 @@
   ...     vroom.Job(1, location=(2.44, 48.81)),
   ...     vroom.Job(2, location=(2.46, 48.7)),
   ...     vroom.Job(3, location=(2.42, 48.6)),
   ... ])
 
   >>> sol = problem_instance.solve(exploration_level=5, nb_threads=4)
   >>> print(sol.summary.duration)
-  2698
+  2704
 
 Installation
 ------------
 
 Pyvroom currently makes binaries for on macOS and Linux. There is also a
 Windows build that can be used, but it is somewhat experimental.
```

### Comparing `pyvroom-1.13.5.dev0/README.rst` & `pyvroom-1.13.5.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pyvroom
+Version: 1.13.5.dev1
+Summary: Vehicle routing open-source optimization machine (VROOM)
+Author: Jonathan Feinberg
+Author-email: jonathf@gmail.com
+License: BSD 2-Clause License
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+
 Python Vehicle Routing Open-source Optimization Machine
 =======================================================
 
 |gh_action| |codecov| |pypi|
 
 .. |gh_action| image:: https://img.shields.io/github/checks-status/VROOM-Project/pyvroom/main
     :target: https://github.com/VROOM-Project/pyvroom/actions
@@ -92,15 +107,15 @@
   ...     vroom.Job(1, location=(2.44, 48.81)),
   ...     vroom.Job(2, location=(2.46, 48.7)),
   ...     vroom.Job(3, location=(2.42, 48.6)),
   ... ])
 
   >>> sol = problem_instance.solve(exploration_level=5, nb_threads=4)
   >>> print(sol.summary.duration)
-  2698
+  2704
 
 Installation
 ------------
 
 Pyvroom currently makes binaries for on macOS and Linux. There is also a
 Windows build that can be used, but it is somewhat experimental.
```

### Comparing `pyvroom-1.13.5.dev0/pyproject.toml` & `pyvroom-1.13.5.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/setup.cfg` & `pyvroom-1.13.5.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/setup.py` & `pyvroom-1.13.5.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/_vroom.cpp` & `pyvroom-1.13.5.dev1/src/_vroom.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/_main.cpp` & `pyvroom-1.13.5.dev1/src/bind/_main.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/amount.cpp` & `pyvroom-1.13.5.dev1/src/bind/amount.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/break.cpp` & `pyvroom-1.13.5.dev1/src/bind/break.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/enums.cpp` & `pyvroom-1.13.5.dev1/src/bind/enums.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/generic/matrix.cpp` & `pyvroom-1.13.5.dev1/src/bind/generic/matrix.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/input/input.cpp` & `pyvroom-1.13.5.dev1/src/bind/input/input.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/input/vehicle_step.cpp` & `pyvroom-1.13.5.dev1/src/bind/input/vehicle_step.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/job.cpp` & `pyvroom-1.13.5.dev1/src/bind/job.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/location.cpp` & `pyvroom-1.13.5.dev1/src/bind/location.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/solution/route.cpp` & `pyvroom-1.13.5.dev1/src/bind/solution/route.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/solution/solution.cpp` & `pyvroom-1.13.5.dev1/src/bind/solution/solution.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -86,26 +86,33 @@
                                 step.step_type == vroom::STEP_TYPE::BREAK)
                                    ? step.id
                                    : NA_SUBSTITUTE;
 
                  ptr[idx].setup = step.setup;
                  ptr[idx].service = step.service;
                  ptr[idx].waiting_time = step.waiting_time;
+                 ptr[idx].distance = step.distance;
                  ptr[idx].arrival = step.arrival;
                  ptr[idx].duration = step.duration;
 
                  idx++;
                }
              }
              return arr;
            })
       .def("_solution_json",
            [](vroom::Solution solution) {
              py::scoped_ostream_redirect stream(
                  std::cout, py::module_::import("sys").attr("stdout"));
+             vroom::io::write_to_json(solution, false, "");
+           })
+      .def("_geometry_solution_json",
+           [](vroom::Solution solution) {
+             py::scoped_ostream_redirect stream(
+                 std::cout, py::module_::import("sys").attr("stdout"));
              vroom::io::write_to_json(solution, true, "");
            })
       .def_readwrite("code", &vroom::Solution::code)
       .def_readwrite("error", &vroom::Solution::error)
       .def_readonly("summary", &vroom::Solution::summary)
       .def_readonly("_routes", &vroom::Solution::routes)
       .def_readonly("unassigned", &vroom::Solution::unassigned);
```

### Comparing `pyvroom-1.13.5.dev0/src/bind/solution/step.cpp` & `pyvroom-1.13.5.dev1/src/bind/solution/step.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/solution/summary.cpp` & `pyvroom-1.13.5.dev1/src/bind/solution/summary.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/time_window.cpp` & `pyvroom-1.13.5.dev1/src/bind/time_window.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/bind/vehicle.cpp` & `pyvroom-1.13.5.dev1/src/bind/vehicle.cpp`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/pyvroom.egg-info/PKG-INFO` & `pyvroom-1.13.5.dev1/src/pyvroom.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvroom
-Version: 1.13.5.dev0
+Version: 1.13.5.dev1
 Summary: Vehicle routing open-source optimization machine (VROOM)
 Author: Jonathan Feinberg
 Author-email: jonathf@gmail.com
 License: BSD 2-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -107,15 +107,15 @@
   ...     vroom.Job(1, location=(2.44, 48.81)),
   ...     vroom.Job(2, location=(2.46, 48.7)),
   ...     vroom.Job(3, location=(2.42, 48.6)),
   ... ])
 
   >>> sol = problem_instance.solve(exploration_level=5, nb_threads=4)
   >>> print(sol.summary.duration)
-  2698
+  2704
 
 Installation
 ------------
 
 Pyvroom currently makes binaries for on macOS and Linux. There is also a
 Windows build that can be used, but it is somewhat experimental.
```

### Comparing `pyvroom-1.13.5.dev0/src/pyvroom.egg-info/SOURCES.txt` & `pyvroom-1.13.5.dev1/src/pyvroom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/vroom/__init__.py` & `pyvroom-1.13.5.dev1/src/vroom/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/vroom/amount.py` & `pyvroom-1.13.5.dev1/src/vroom/amount.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/vroom/break_.py` & `pyvroom-1.13.5.dev1/src/vroom/break_.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/vroom/input/forced_service.py` & `pyvroom-1.13.5.dev1/src/vroom/input/forced_service.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/vroom/input/input.py` & `pyvroom-1.13.5.dev1/src/vroom/input/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         jobs:
             Jobs that needs to be completed in the routing problem.
         vehicles:
             Vehicles available to solve the routing problem.
 
     """
 
+    _geometry: bool = False
+
     def __init__(
         self,
         amount_size: Optional[int] = None,
         servers: Optional[Dict[str, Union[str, _vroom.Server]]] = None,
         router: _vroom.ROUTER = _vroom.ROUTER.OSRM,
     ) -> None:
         """Class initializer.
@@ -100,21 +102,24 @@
 
         Returns:
             Input instance with all jobs, shipments, etc. added from JSON.
 
         """
         if geometry is None:
             geometry = servers is not None
+        if geometry:
+            self._set_geometry(True)
         instance = Input(servers=servers, router=router)
         with open(filepath) as handle:
             instance._from_json(handle.read(), geometry)
         return instance
 
     def set_geometry(self):
-        return self._set_geometry()
+        self._geometry = True
+        return self._set_geometry(True)
 
     def set_amount_size(self, *amount_sizes: int) -> None:
         """Add amount sizes."""
         sizes = set(amount_sizes)
         if self._amount_size is not None:
             sizes.add(self._amount_size)
         if len(sizes) > 1:
@@ -303,13 +308,16 @@
         self._set_costs_matrix(profile, matrix_input)
 
     def solve(
         self,
         exploration_level: int,
         nb_threads: int,
     ) -> Solution:
-        return Solution(
+        solution = Solution(
             self._solve(
                 exploration_level=exploration_level,
                 nb_threads=nb_threads,
             )
+
         )
+        solution._geometry = self._geometry
+        return solution
```

### Comparing `pyvroom-1.13.5.dev0/src/vroom/input/vehicle_step.py` & `pyvroom-1.13.5.dev1/src/vroom/input/vehicle_step.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/vroom/job.py` & `pyvroom-1.13.5.dev1/src/vroom/job.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/vroom/location.py` & `pyvroom-1.13.5.dev1/src/vroom/location.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/vroom/solution/solution.py` & `pyvroom-1.13.5.dev1/src/vroom/solution/solution.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     The computed solutions.
 
     Attributes:
         routes:
             Frame outlining all routes for all vehicles.
     """
 
+    _geometry: bool = False
+
     @property
     def routes(self) -> pandas.DataFrame:
         """
         Frame outlining all routes for all vehicles.
 
         It includes the following columns.
 
@@ -77,21 +79,29 @@
             }
         )
         for column in ["longitude", "latitude", "id"]:
             if (frame[column] == NA_SUBSTITUTE).all():
                 del frame[column]
             else:
                 frame.loc[frame[column] == NA_SUBSTITUTE, column] = pandas.NA
+        if self._geometry:
+            frame["distance"] = array["distance"]
         return frame
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert solution into VROOM compatible dictionary."""
         stream = io.StringIO()
         with redirect_stdout(stream):
-            self._solution_json()
+            if self._geometry:
+                self._geometry_solution_json()
+            else:
+                self._solution_json()
         return json.loads(stream.getvalue())
 
     def to_json(self, filepath: Union[str, Path]) -> None:
         """Store solution into VROOM compatible JSON file."""
         with open(filepath, "w") as handler:
             with redirect_stdout(handler):
-                self._solution_json()
+                if self._geometry:
+                    self._geometry_solution_json()
+                else:
+                    self._solution_json()
```

### Comparing `pyvroom-1.13.5.dev0/src/vroom/time_window.py` & `pyvroom-1.13.5.dev1/src/vroom/time_window.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/src/vroom/vehicle.py` & `pyvroom-1.13.5.dev1/src/vroom/vehicle.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/test/input/test_vehicle_step.py` & `pyvroom-1.13.5.dev1/test/input/test_vehicle_step.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/test/test_amount.py` & `pyvroom-1.13.5.dev1/test/test_amount.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/test/test_break.py` & `pyvroom-1.13.5.dev1/test/test_break.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/test/test_file_handle.py` & `pyvroom-1.13.5.dev1/test/test_file_handle.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/test/test_job.py` & `pyvroom-1.13.5.dev1/test/test_job.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/test/test_libvroom_examples.py` & `pyvroom-1.13.5.dev1/test/test_libvroom_examples.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/test/test_location.py` & `pyvroom-1.13.5.dev1/test/test_location.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/test/test_time_window.py` & `pyvroom-1.13.5.dev1/test/test_time_window.py`

 * *Files identical despite different names*

### Comparing `pyvroom-1.13.5.dev0/test/test_vehicle.py` & `pyvroom-1.13.5.dev1/test/test_vehicle.py`

 * *Files identical despite different names*

