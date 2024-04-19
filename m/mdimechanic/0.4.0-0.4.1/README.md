# Comparing `tmp/mdimechanic-0.4.0.tar.gz` & `tmp/mdimechanic-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdimechanic-0.4.0.tar", last modified: Thu Mar  7 18:39:15 2024, max compression
+gzip compressed data, was "mdimechanic-0.4.1.tar", last modified: Fri Apr 19 13:44:52 2024, max compression
```

## Comparing `mdimechanic-0.4.0.tar` & `mdimechanic-0.4.1.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.262528 mdimechanic-0.4.0/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     1459 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/LICENSE
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      118 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/MANIFEST.in
--rw-r--r--   0 taylor    (1001) taylor    (1001)     1080 2024-03-07 18:39:15.262528 mdimechanic-0.4.0/PKG-INFO
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      667 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/README.md
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      311 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/__init__.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)       47 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/__main__.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)    18453 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/_version.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     2588 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/cli.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     4734 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/cmd_build.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     2974 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/cmd_interactive.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     4179 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/cmd_report.py
--rwxrwxr-x   0 taylor    (1001) taylor    (1001)     4905 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/cmd_run.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     3438 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/cmd_rundriver.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     3135 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/commands.py
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/data/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     1139 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/data/README.md
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      333 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/data/look_and_say.dat
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/docker/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      524 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/Dockerfile
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/docker/base/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     2905 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/base/Dockerfile
--rwxrwxr-x   0 taylor    (1001) taylor    (1001)      524 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/base/docker-entrypoint.sh
--rwxrwxr-x   0 taylor    (1001) taylor    (1001)       57 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/clean.sh
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/docker/mpi/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      558 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/mpi/docker-compose.yml
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      149 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/mpi/mdi_appfile
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/docker/mpi_nvidia/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      716 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/mpi_nvidia/docker-compose.yml
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      149 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/mpi_nvidia/mdi_appfile
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/docker/run/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      373 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/run/docker-compose.yml
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/docker/run_nvidia/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      531 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/run_nvidia/docker-compose.yml
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/docker/ssh/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)       25 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/ssh/config
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/docker/tcp/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      717 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/tcp/docker-compose.yml
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/docker/tcp_nvidia/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      875 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/docker/tcp_nvidia/docker-compose.yml
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/drivers/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     5052 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/drivers/min_driver.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     2434 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/mdi_standard.yaml
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/projects/
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/projects/enginereport/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     2007 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/projects/enginereport/.gitignore
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/projects/enginereport/docker/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      274 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/projects/enginereport/docker/Dockerfile
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      619 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/projects/enginereport/mdimechanic.yml
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/report/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     2289 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/README.base
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.258528 mdimechanic-0.4.0/mdimechanic/report/base_report/
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.262528 mdimechanic-0.4.0/mdimechanic/report/base_report/badges/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      830 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/badges/-failing-red.svg
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      824 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/badges/-working-success.svg
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      644 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-blue.svg
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      638 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-brightgreen.svg
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      644 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-green.svg
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      644 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-lightgray.svg
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      644 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-orange.svg
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      644 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-red.svg
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      644 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-yellow.svg
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      644 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-yellowgreen.svg
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.262528 mdimechanic-0.4.0/mdimechanic/report/base_report/dynamic_badges/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      830 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/dynamic_badges/step_engine_build.svg
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      830 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/dynamic_badges/step_mdi_nodes.svg
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      830 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/dynamic_badges/step_min_engine.svg
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      830 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/dynamic_badges/step_unsupported.svg
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.262528 mdimechanic-0.4.0/mdimechanic/report/base_report/graphs/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      830 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/graphs/node-report.gv.svg
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.262528 mdimechanic-0.4.0/mdimechanic/report/base_report/markdown/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      789 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/markdown/minimalistic.md
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      123 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/report/base_report/markdown/validation.md
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.262528 mdimechanic-0.4.0/mdimechanic/tests/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      112 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/tests/__init__.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      316 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/tests/test_mdimechanic.py
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.262528 mdimechanic-0.4.0/mdimechanic/utils/
--rw-rw-r--   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/utils/__init__.py
--rwxrwxr-x   0 taylor    (1001) taylor    (1001)      100 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/utils/generate_ssh_keys.sh
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      842 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/utils/graph.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)    17437 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/utils/node_analysis.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     1271 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/utils/parse_standard.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     2642 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/utils/reset_report.py
--rwxrwxr-x   0 taylor    (1001) taylor    (1001)     8510 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/utils/tests.py
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     3283 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/mdimechanic/utils/utils.py
-drwxrwxr-x   0 taylor    (1001) taylor    (1001)        0 2024-03-07 18:39:15.262528 mdimechanic-0.4.0/mdimechanic.egg-info/
--rw-r--r--   0 taylor    (1001) taylor    (1001)     1080 2024-03-07 18:39:15.000000 mdimechanic-0.4.0/mdimechanic.egg-info/PKG-INFO
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     2671 2024-03-07 18:39:15.000000 mdimechanic-0.4.0/mdimechanic.egg-info/SOURCES.txt
--rw-rw-r--   0 taylor    (1001) taylor    (1001)        1 2024-03-07 18:39:15.000000 mdimechanic-0.4.0/mdimechanic.egg-info/dependency_links.txt
--rw-rw-r--   0 taylor    (1001) taylor    (1001)       53 2024-03-07 18:39:15.000000 mdimechanic-0.4.0/mdimechanic.egg-info/entry_points.txt
--rw-rw-r--   0 taylor    (1001) taylor    (1001)        1 2024-03-07 18:39:15.000000 mdimechanic-0.4.0/mdimechanic.egg-info/not-zip-safe
--rw-rw-r--   0 taylor    (1001) taylor    (1001)       48 2024-03-07 18:39:15.000000 mdimechanic-0.4.0/mdimechanic.egg-info/requires.txt
--rw-rw-r--   0 taylor    (1001) taylor    (1001)       12 2024-03-07 18:39:15.000000 mdimechanic-0.4.0/mdimechanic.egg-info/top_level.txt
--rw-rw-r--   0 taylor    (1001) taylor    (1001)     3077 2024-03-07 18:38:59.000000 mdimechanic-0.4.0/pyproject.toml
--rw-rw-r--   0 taylor    (1001) taylor    (1001)      360 2024-03-07 18:39:15.262528 mdimechanic-0.4.0/setup.cfg
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     1459 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/LICENSE
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      118 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/MANIFEST.in
+-rw-r--r--   0 taylor    (1000) taylor    (1000)     1080 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/PKG-INFO
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      667 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/README.md
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.690504 mdimechanic-0.4.1/mdimechanic/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      311 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/__init__.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)       47 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/__main__.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)    18453 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/_version.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     2643 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/cli.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     4734 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/cmd_build.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     2974 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/cmd_interactive.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     4230 2024-04-19 13:43:07.000000 mdimechanic-0.4.1/mdimechanic/cmd_report.py
+-rwxrwxr-x   0 taylor    (1000) taylor    (1000)     4957 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/cmd_run.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     3490 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/cmd_rundriver.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     3135 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/commands.py
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/data/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     1139 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/data/README.md
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      333 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/data/look_and_say.dat
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/docker/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      524 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/Dockerfile
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/docker/base/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     2905 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/base/Dockerfile
+-rwxrwxr-x   0 taylor    (1000) taylor    (1000)      524 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/base/docker-entrypoint.sh
+-rwxrwxr-x   0 taylor    (1000) taylor    (1000)       57 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/clean.sh
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/docker/mpi/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      558 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/mpi/docker-compose.yml
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      149 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/mpi/mdi_appfile
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/docker/mpi_nvidia/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      716 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/mpi_nvidia/docker-compose.yml
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      149 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/mpi_nvidia/mdi_appfile
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/docker/run/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      373 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/run/docker-compose.yml
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/docker/run_nvidia/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      531 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/run_nvidia/docker-compose.yml
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/docker/ssh/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)       25 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/ssh/config
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/docker/tcp/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      717 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/tcp/docker-compose.yml
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/docker/tcp_nvidia/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      875 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/docker/tcp_nvidia/docker-compose.yml
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/drivers/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     5052 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/drivers/min_driver.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     2434 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/mdi_standard.yaml
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.690504 mdimechanic-0.4.1/mdimechanic/projects/
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/projects/enginereport/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     2007 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/projects/enginereport/.gitignore
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/projects/enginereport/docker/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      274 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/projects/enginereport/docker/Dockerfile
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      619 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/projects/enginereport/mdimechanic.yml
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/report/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     2289 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/README.base
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.690504 mdimechanic-0.4.1/mdimechanic/report/base_report/
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/report/base_report/badges/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      830 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/badges/-failing-red.svg
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      824 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/badges/-working-success.svg
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      644 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-blue.svg
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      638 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-brightgreen.svg
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      644 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-green.svg
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      644 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-lightgray.svg
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      644 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-orange.svg
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      644 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-red.svg
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      644 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-yellow.svg
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      644 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-yellowgreen.svg
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/report/base_report/dynamic_badges/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      830 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/dynamic_badges/step_engine_build.svg
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      830 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/dynamic_badges/step_mdi_nodes.svg
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      830 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/dynamic_badges/step_min_engine.svg
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      830 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/dynamic_badges/step_unsupported.svg
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/report/base_report/graphs/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      830 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/graphs/node-report.gv.svg
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/report/base_report/markdown/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      789 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/markdown/minimalistic.md
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      123 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/report/base_report/markdown/validation.md
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/tests/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      112 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/tests/__init__.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      316 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/tests/test_mdimechanic.py
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic/utils/
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)        0 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/utils/__init__.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      842 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/utils/determine_compose.py
+-rwxrwxr-x   0 taylor    (1000) taylor    (1000)      100 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/utils/generate_ssh_keys.sh
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      842 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/utils/graph.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)    17483 2024-04-19 13:43:07.000000 mdimechanic-0.4.1/mdimechanic/utils/node_analysis.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     1271 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/utils/parse_standard.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     2642 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/utils/reset_report.py
+-rwxrwxr-x   0 taylor    (1000) taylor    (1000)     8556 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/utils/tests.py
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     3283 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/mdimechanic/utils/utils.py
+drwxrwxr-x   0 taylor    (1000) taylor    (1000)        0 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/mdimechanic.egg-info/
+-rw-r--r--   0 taylor    (1000) taylor    (1000)     1080 2024-04-19 13:44:52.000000 mdimechanic-0.4.1/mdimechanic.egg-info/PKG-INFO
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     2710 2024-04-19 13:44:52.000000 mdimechanic-0.4.1/mdimechanic.egg-info/SOURCES.txt
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)        1 2024-04-19 13:44:52.000000 mdimechanic-0.4.1/mdimechanic.egg-info/dependency_links.txt
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)       53 2024-04-19 13:44:52.000000 mdimechanic-0.4.1/mdimechanic.egg-info/entry_points.txt
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)        1 2024-04-18 16:27:18.000000 mdimechanic-0.4.1/mdimechanic.egg-info/not-zip-safe
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)       48 2024-04-19 13:44:52.000000 mdimechanic-0.4.1/mdimechanic.egg-info/requires.txt
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)       12 2024-04-19 13:44:52.000000 mdimechanic-0.4.1/mdimechanic.egg-info/top_level.txt
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)     3077 2024-04-18 16:27:10.000000 mdimechanic-0.4.1/pyproject.toml
+-rw-rw-r--   0 taylor    (1000) taylor    (1000)      360 2024-04-19 13:44:52.694504 mdimechanic-0.4.1/setup.cfg
```

### Comparing `mdimechanic-0.4.0/LICENSE` & `mdimechanic-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/PKG-INFO` & `mdimechanic-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdimechanic
-Version: 0.4.0
+Version: 0.4.1
 Summary: A tool for testing and developing MDI-enabled projects.
 Author-email: Taylor Barnes <mdi@molssi.org>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML>=5.0
```

### Comparing `mdimechanic-0.4.0/README.md` & `mdimechanic-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/_version.py` & `mdimechanic-0.4.1/mdimechanic/_version.py`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/cli.py` & `mdimechanic-0.4.1/mdimechanic/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Provides a CLI for MDI_Mechanic
 """
 
 import argparse
+import subprocess
 import sys
 from . import commands
 
+from .utils import utils as ut
+
 def parse_args():
     parser = argparse.ArgumentParser(description="A CLI for the MDI_Mechanic.")
 
     subparsers = parser.add_subparsers(dest="command")
 
     build = subparsers.add_parser("build", help="Build containers for MDI_Mechanic and the engine.")
     #build.add_argument("location", type=str, help="The location where the engine is located.")
@@ -47,14 +50,15 @@
     if args["command"] is None:
         parser.print_help(sys.stderr)
         exit(1)
 
     return args
 
 def main(args=None):
+    
     if args is None:
         args = parse_args()
 
     command = args.pop("command")
     if command == "build":
         commands.command_build( args )
     elif command == "report":
```

### Comparing `mdimechanic-0.4.0/mdimechanic/cmd_build.py` & `mdimechanic-0.4.1/mdimechanic/cmd_build.py`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/cmd_interactive.py` & `mdimechanic-0.4.1/mdimechanic/cmd_interactive.py`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/cmd_report.py` & `mdimechanic-0.4.1/mdimechanic/cmd_report.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import subprocess
 from shutil import copyfile
 from .utils import tests as mtests
 from .utils import node_analysis as na
 from .utils import reset_report as rr
 from .utils import utils as ut
+from .utils.determine_compose import COMPOSE_COMMAND
 
 # Generate the report
 def generate_report( base_path ):
 
     # Path to this file
     #file_path = os.path.dirname(os.path.realpath(__file__))
 
@@ -17,23 +18,23 @@
 
     # Reset the report
     rr.reset_report( base_path )
 
     # Ensure that there are no orphaned containers / networks running
     try:
         compose_path = ut.get_compose_path( "tcp" )
-        down_proc = subprocess.Popen( ["docker-compose", "down"],
+        down_proc = subprocess.Popen(COMPOSE_COMMAND + ["down"],
                                       stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                       cwd=compose_path)
         down_tup = down_proc.communicate()
     except:
         raise Exception("Error: Unable to remove orphaned containers.")
     try:
         compose_path = ut.get_compose_path( "tcp_nvidia" )
-        down_proc = subprocess.Popen( ["docker-compose", "down"],
+        down_proc = subprocess.Popen(COMPOSE_COMMAND + ["down"],
                                       stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                       cwd=compose_path)
         down_tup = down_proc.communicate()
     except:
         raise Exception("Error: Unable to remove orphaned containers.")
 
     # Verify that the engine has been built / installed correctly
```

### Comparing `mdimechanic-0.4.0/mdimechanic/cmd_run.py` & `mdimechanic-0.4.1/mdimechanic/cmd_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import subprocess
 import shutil
 from .utils.utils import format_return, insert_list, docker_error, get_mdi_standard, get_compose_path, get_package_path, get_mdimechanic_yaml, write_as_bytes
-
+from .utils.determine_compose import COMPOSE_COMMAND
 
 def run( script_name, base_path ):
     mdimechanic_yaml = get_mdimechanic_yaml( base_path )
 
     # Get the path to the docker-compose file
     docker_path = os.path.join( base_path, ".mdimechanic", ".temp" )
 
@@ -91,23 +91,23 @@
         script_file_name = "docker_mdi_" + str(icontainer) + ".sh"
         script_path = os.path.join( base_path, ".mdimechanic", ".temp", script_file_name )
         os.makedirs(os.path.dirname(script_path), exist_ok=True)
         write_as_bytes( script, script_path )
 
     # Launch with docker-compose
     docker_env = os.environ
-    up_proc = subprocess.Popen( ["docker-compose", "up"],
+    up_proc = subprocess.Popen( COMPOSE_COMMAND + ["up"],
                                 stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                 cwd=docker_path, env=docker_env )
     up_tup = up_proc.communicate()
     up_out = format_return(up_tup[0])
     up_err = format_return(up_tup[1])
 
     # Run "docker-compose down"
-    down_proc = subprocess.Popen( ["docker-compose", "down"],
+    down_proc = subprocess.Popen( COMPOSE_COMMAND + ["down"],
                                 stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                   cwd=docker_path, env=docker_env )
     down_tup = down_proc.communicate()
     down_out = format_return(down_tup[0])
     down_err = format_return(down_tup[1])
 
     if up_proc.returncode != 0:
```

### Comparing `mdimechanic-0.4.0/mdimechanic/cmd_rundriver.py` & `mdimechanic-0.4.1/mdimechanic/cmd_rundriver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import subprocess
 import shutil
 from .utils.utils import format_return, insert_list, docker_error, get_mdi_standard, get_compose_path, get_package_path, get_mdimechanic_yaml, writelines_as_bytes, write_as_bytes
-
+from .utils.determine_compose import COMPOSE_COMMAND
 
 def test_driver( driver_name, base_path ):
     mdimechanic_yaml = get_mdimechanic_yaml( base_path )
 
     # Get the path to the docker-compose file
     docker_path = None
     if 'gpu' in mdimechanic_yaml['docker']:
@@ -43,24 +43,24 @@
     # Create the docker environment
     docker_env = os.environ
     docker_env['MDIMECH_WORKDIR'] = base_path
     docker_env['MDIMECH_PACKAGEDIR'] = get_package_path()
     docker_env['MDIMECH_ENGINE_NAME'] = mdimechanic_yaml['docker']['image_name'] + ":dev"
 
     # Run "docker-compose up"
-    up_proc = subprocess.Popen( ["docker-compose", "up", "--exit-code-from", "mdi_mechanic", "--abort-on-container-exit"],
+    up_proc = subprocess.Popen( COMPOSE_COMMAND + ["up", "--exit-code-from", "mdi_mechanic", "--abort-on-container-exit"],
                                 stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                 cwd=docker_path, env=docker_env )
     up_tup = up_proc.communicate()
     up_out = format_return(up_tup[0])
     up_err = format_return(up_tup[1])
 
 
     # Run "docker-compose down"
-    down_proc = subprocess.Popen( ["docker-compose", "down"],
+    down_proc = subprocess.Popen( COMPOSE_COMMAND + ["down"],
                                 stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                   cwd=docker_path, env=docker_env )
     down_tup = down_proc.communicate()
     down_out = format_return(down_tup[0])
     down_err = format_return(down_tup[1])
 
     if up_proc.returncode != 0:
```

### Comparing `mdimechanic-0.4.0/mdimechanic/commands.py` & `mdimechanic-0.4.1/mdimechanic/commands.py`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/data/README.md` & `mdimechanic-0.4.1/mdimechanic/data/README.md`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/docker/Dockerfile` & `mdimechanic-0.4.1/mdimechanic/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/docker/base/Dockerfile` & `mdimechanic-0.4.1/mdimechanic/docker/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/docker/base/docker-entrypoint.sh` & `mdimechanic-0.4.1/mdimechanic/docker/base/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/docker/mpi/docker-compose.yml` & `mdimechanic-0.4.1/mdimechanic/docker/mpi/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/docker/mpi_nvidia/docker-compose.yml` & `mdimechanic-0.4.1/mdimechanic/docker/mpi_nvidia/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/docker/run_nvidia/docker-compose.yml` & `mdimechanic-0.4.1/mdimechanic/docker/run_nvidia/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/docker/tcp/docker-compose.yml` & `mdimechanic-0.4.1/mdimechanic/docker/tcp/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/docker/tcp_nvidia/docker-compose.yml` & `mdimechanic-0.4.1/mdimechanic/docker/tcp_nvidia/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/drivers/min_driver.py` & `mdimechanic-0.4.1/mdimechanic/drivers/min_driver.py`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/mdi_standard.yaml` & `mdimechanic-0.4.1/mdimechanic/mdi_standard.yaml`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/projects/enginereport/.gitignore` & `mdimechanic-0.4.1/mdimechanic/projects/enginereport/.gitignore`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/projects/enginereport/mdimechanic.yml` & `mdimechanic-0.4.1/mdimechanic/projects/enginereport/mdimechanic.yml`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/README.base` & `mdimechanic-0.4.1/mdimechanic/report/README.base`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/badges/-failing-red.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/badges/-failing-red.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/badges/-working-success.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/badges/-working-success.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-blue.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-blue.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-brightgreen.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-brightgreen.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-green.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-green.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-lightgray.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-lightgray.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-orange.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-orange.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-red.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-red.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-yellow.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-yellow.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/badges/box-yellowgreen.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/badges/box-yellowgreen.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/dynamic_badges/step_engine_build.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/dynamic_badges/step_engine_build.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/dynamic_badges/step_mdi_nodes.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/dynamic_badges/step_mdi_nodes.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/dynamic_badges/step_min_engine.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/dynamic_badges/step_min_engine.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/dynamic_badges/step_unsupported.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/dynamic_badges/step_unsupported.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/graphs/node-report.gv.svg` & `mdimechanic-0.4.1/mdimechanic/report/base_report/graphs/node-report.gv.svg`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/report/base_report/markdown/minimalistic.md` & `mdimechanic-0.4.1/mdimechanic/report/base_report/markdown/minimalistic.md`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/utils/graph.py` & `mdimechanic-0.4.1/mdimechanic/utils/graph.py`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/utils/node_analysis.py` & `mdimechanic-0.4.1/mdimechanic/utils/node_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import sys
 import subprocess
 import pickle
 from .utils import format_return, insert_list, docker_error, get_mdi_standard, get_compose_path, get_package_path, get_mdimechanic_yaml, writelines_as_bytes, write_as_bytes
+from .determine_compose import COMPOSE_COMMAND
 
 # Paths to enter each identified node
 node_paths = { "@DEFAULT": "" }
 
 # Paths associated with the edges for the node graph
 node_edge_paths = [ ("@DEFAULT", "") ]
 
@@ -19,30 +20,30 @@
     # Create the docker environment
     docker_env = os.environ
     docker_env['MDIMECH_WORKDIR'] = base_path
     docker_env['MDIMECH_PACKAGEDIR'] = get_package_path()
     docker_env['MDIMECH_ENGINE_NAME'] = mdimechanic_yaml['docker']['image_name'] + ":dev"
 
     # Run "docker-compose up -d"
-    up_proc = subprocess.Popen( ["docker-compose", "up", "-d"],
+    up_proc = subprocess.Popen( COMPOSE_COMMAND + ["up", "-d"],
                                 stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                 cwd=docker_path, env=docker_env )
     up_tup = up_proc.communicate()
     up_out = format_return(up_tup[0])
     up_err = format_return(up_tup[1])
     return up_proc.returncode
 
 def docker_down( base_path, docker_path ):
     # Create the docker environment
     docker_env = os.environ
     docker_env['MDIMECH_WORKDIR'] = base_path
     docker_env['MDIMECH_PACKAGEDIR'] = get_package_path()
 
     # Run "docker-compose down"
-    down_proc = subprocess.Popen( ["docker-compose", "down"],
+    down_proc = subprocess.Popen( COMPOSE_COMMAND + ["down"],
                                   stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                   cwd=docker_path, env=docker_env )
     down_tup = down_proc.communicate()
     down_out = format_return(down_tup[0])
     down_err = format_return(down_tup[1])
     return down_proc.returncode
 
@@ -118,15 +119,15 @@
         # Create the docker environment
         docker_env = os.environ
         docker_env['MDIMECH_WORKDIR'] = base_path
         docker_env['MDIMECH_PACKAGEDIR'] = get_package_path()
         docker_env['MDIMECH_ENGINE_NAME'] = mdimechanic_yaml['docker']['image_name'] + ":dev"
 
         # Run "docker-compose exec"
-        exec_proc = subprocess.Popen( ["docker-compose", "exec", "-T", "--user", "mpiuser", "mdi_mechanic", "mpiexec", "-app", "/MDI_Mechanic/mdimechanic/docker/mpi/mdi_appfile"],
+        exec_proc = subprocess.Popen( COMPOSE_COMMAND + ["exec", "-T", "--user", "mpiuser", "mdi_mechanic", "mpiexec", "-app", "/MDI_Mechanic/mdimechanic/docker/mpi/mdi_appfile"],
                                       stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                       cwd=docker_path, env=docker_env )
         exec_tup = exec_proc.communicate()
         exec_out = format_return(exec_tup[0])
         exec_err = format_return(exec_tup[1])
         if exec_proc.returncode != 0:
             print("FAILED", flush=True)
@@ -138,15 +139,15 @@
         # Create the docker environment
         docker_env = os.environ
         docker_env['MDIMECH_WORKDIR'] = base_path
         docker_env['MDIMECH_PACKAGEDIR'] = get_package_path()
         docker_env['MDIMECH_ENGINE_NAME'] = mdimechanic_yaml['docker']['image_name'] + ":dev"
 
         # Run the docker container
-        up_proc = subprocess.Popen( ["docker-compose", "up", "--exit-code-from", "mdi_mechanic", "--abort-on-container-exit"],
+        up_proc = subprocess.Popen(COMPOSE_COMMAND + ["up", "--exit-code-from", "mdi_mechanic", "--abort-on-container-exit"],
                                     stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                     cwd=docker_path, env=docker_env )
         up_tup = up_proc.communicate()
         up_out = format_return(up_tup[0])
         up_err = format_return(up_tup[1])
         if up_proc.returncode != 0:
             print("FAILED", flush=True)
```

### Comparing `mdimechanic-0.4.0/mdimechanic/utils/parse_standard.py` & `mdimechanic-0.4.1/mdimechanic/utils/parse_standard.py`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/utils/reset_report.py` & `mdimechanic-0.4.1/mdimechanic/utils/reset_report.py`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic/utils/tests.py` & `mdimechanic-0.4.1/mdimechanic/utils/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import subprocess
 import shutil
 from .utils import format_return, insert_list, docker_error, get_mdi_standard, get_compose_path, get_package_path, get_mdimechanic_yaml, writelines_as_bytes, write_as_bytes
-
+from .determine_compose import COMPOSE_COMMAND
 
 
 def test_validate( base_path ):
     # Get the base directory
     package_path = get_package_path()
 
     # Get the MDI YAML
@@ -79,23 +79,23 @@
     # Create the docker environment
     docker_env = os.environ
     docker_env['MDIMECH_WORKDIR'] = base_path
     docker_env['MDIMECH_PACKAGEDIR'] = get_package_path()
     docker_env['MDIMECH_ENGINE_NAME'] = mdimechanic_yaml['docker']['image_name'] + ":dev"
 
     # Run "docker-compose up"
-    up_proc = subprocess.Popen( ["docker-compose", "up", "--exit-code-from", "mdi_mechanic", "--abort-on-container-exit"],
+    up_proc = subprocess.Popen( COMPOSE_COMMAND + ["up", "--exit-code-from", "mdi_mechanic", "--abort-on-container-exit"],
                                 stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                 cwd=docker_path, env=docker_env )
     up_tup = up_proc.communicate()
     up_out = format_return(up_tup[0])
     up_err = format_return(up_tup[1])
 
     # Run "docker-compose down"
-    down_proc = subprocess.Popen( ["docker-compose", "down"],
+    down_proc = subprocess.Popen( COMPOSE_COMMAND + ["down"],
                                 stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                   cwd=docker_path, env=docker_env )
     down_tup = down_proc.communicate()
     down_out = format_return(down_tup[0])
     down_err = format_return(down_tup[1])
 
     if up_proc.returncode != 0:
@@ -152,23 +152,23 @@
     # Create the docker environment
     docker_env = os.environ
     docker_env['MDIMECH_WORKDIR'] = base_path
     docker_env['MDIMECH_PACKAGEDIR'] = get_package_path()
     docker_env['MDIMECH_ENGINE_NAME'] = mdimechanic_yaml['docker']['image_name'] + ":dev"
 
     # Run "docker-compose up"
-    up_proc = subprocess.Popen( ["docker-compose", "up", "--exit-code-from", "mdi_mechanic", "--abort-on-container-exit"],
+    up_proc = subprocess.Popen( COMPOSE_COMMAND + ["up", "--exit-code-from", "mdi_mechanic", "--abort-on-container-exit"],
                                 stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                 cwd=docker_path, env=docker_env )
     up_tup = up_proc.communicate()
     up_out = format_return(up_tup[0])
     up_err = format_return(up_tup[1])
 
     # Run "docker-compose down"
-    down_proc = subprocess.Popen( ["docker-compose", "down"],
+    down_proc = subprocess.Popen( COMPOSE_COMMAND + ["down"],
                                   stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                                   cwd=docker_path, env=docker_env )
     down_tup = down_proc.communicate()
     down_out = format_return(down_tup[0])
     down_err = format_return(down_tup[1])
 
     #assert up_proc.returncode != 0
```

### Comparing `mdimechanic-0.4.0/mdimechanic/utils/utils.py` & `mdimechanic-0.4.1/mdimechanic/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mdimechanic-0.4.0/mdimechanic.egg-info/PKG-INFO` & `mdimechanic-0.4.1/mdimechanic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdimechanic
-Version: 0.4.0
+Version: 0.4.1
 Summary: A tool for testing and developing MDI-enabled projects.
 Author-email: Taylor Barnes <mdi@molssi.org>
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyYAML>=5.0
```

### Comparing `mdimechanic-0.4.0/mdimechanic.egg-info/SOURCES.txt` & `mdimechanic-0.4.1/mdimechanic.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 mdimechanic/report/base_report/dynamic_badges/step_unsupported.svg
 mdimechanic/report/base_report/graphs/node-report.gv.svg
 mdimechanic/report/base_report/markdown/minimalistic.md
 mdimechanic/report/base_report/markdown/validation.md
 mdimechanic/tests/__init__.py
 mdimechanic/tests/test_mdimechanic.py
 mdimechanic/utils/__init__.py
+mdimechanic/utils/determine_compose.py
 mdimechanic/utils/generate_ssh_keys.sh
 mdimechanic/utils/graph.py
 mdimechanic/utils/node_analysis.py
 mdimechanic/utils/parse_standard.py
 mdimechanic/utils/reset_report.py
 mdimechanic/utils/tests.py
 mdimechanic/utils/utils.py
```

### Comparing `mdimechanic-0.4.0/pyproject.toml` & `mdimechanic-0.4.1/pyproject.toml`

 * *Files identical despite different names*

