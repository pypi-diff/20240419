# Comparing `tmp/pyreports-1.6.0.tar.gz` & `tmp/pyreports-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreports-1.6.0.tar", last modified: Fri Jul 14 09:43:06 2023, max compression
+gzip compressed data, was "pyreports-1.7.0.tar", last modified: Fri Apr 19 08:15:03 2024, max compression
```

## Comparing `pyreports-1.6.0.tar` & `pyreports-1.7.0.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.784167 pyreports-1.6.0/
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.777167 pyreports-1.6.0/.circleci/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      581 2023-07-14 09:39:08.000000 pyreports-1.6.0/.circleci/config.yml
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.777167 pyreports-1.6.0/.github/
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.777167 pyreports-1.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      310 2021-05-22 09:10:30.000000 pyreports-1.6.0/.github/ISSUE_TEMPLATE/reports-enhancement.md
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      350 2021-05-22 09:10:30.000000 pyreports-1.6.0/.github/ISSUE_TEMPLATE/reports-issue.md
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      330 2020-09-16 09:59:48.000000 pyreports-1.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     3272 2021-05-01 12:43:38.000000 pyreports-1.6.0/.gitignore
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     3010 2023-07-14 09:39:08.000000 pyreports-1.6.0/CHANGES.md
--rw-rw-r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     2503 2019-10-29 13:39:34.000000 pyreports-1.6.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     4049 2019-10-28 14:57:18.000000 pyreports-1.6.0/CONTRIBUTING.md
--rwxrwxr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    34916 2019-10-26 09:26:26.000000 pyreports-1.6.0/LICENSE.md
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       22 2023-07-14 09:39:08.000000 pyreports-1.6.0/MANIFEST.in
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     9612 2023-07-14 09:43:06.783167 pyreports-1.6.0/PKG-INFO
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8513 2022-09-27 09:45:00.000000 pyreports-1.6.0/README.md
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.777167 pyreports-1.6.0/assets/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8196 2022-04-15 12:42:38.000000 pyreports-1.6.0/assets/.DS_Store
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.777167 pyreports-1.6.0/assets/css/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     6148 2022-04-15 12:42:38.000000 pyreports-1.6.0/assets/css/.DS_Store
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    12830 2021-05-26 12:03:02.000000 pyreports-1.6.0/assets/css/theme-1.css
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.778167 pyreports-1.6.0/assets/js/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     6148 2022-04-15 12:42:38.000000 pyreports-1.6.0/assets/js/.DS_Store
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      882 2021-05-26 12:03:02.000000 pyreports-1.6.0/assets/js/main.js
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.778167 pyreports-1.6.0/docs/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      638 2021-05-08 08:55:41.000000 pyreports-1.6.0/docs/Makefile
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      764 2021-05-08 08:55:41.000000 pyreports-1.6.0/docs/make.bat
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       80 2022-08-04 10:18:33.000000 pyreports-1.6.0/docs/requirements.txt
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.779167 pyreports-1.6.0/docs/source/
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.779167 pyreports-1.6.0/docs/source/_static/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    14659 2021-05-26 10:37:38.000000 pyreports-1.6.0/docs/source/_static/pyreports.svg
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     2149 2022-07-18 07:37:08.000000 pyreports-1.6.0/docs/source/conf.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     4737 2022-08-04 10:18:33.000000 pyreports-1.6.0/docs/source/datatools.rst
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.780167 pyreports-1.6.0/docs/source/dev/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8840 2023-07-14 09:39:08.000000 pyreports-1.6.0/docs/source/dev/cli.rst
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     5896 2021-05-22 09:10:30.000000 pyreports-1.6.0/docs/source/dev/core.rst
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     3801 2023-07-14 09:39:08.000000 pyreports-1.6.0/docs/source/dev/io.rst
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    11452 2021-05-22 09:10:30.000000 pyreports-1.6.0/docs/source/example.rst
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8402 2021-05-22 09:10:30.000000 pyreports-1.6.0/docs/source/executors.rst
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     2066 2022-08-04 10:18:33.000000 pyreports-1.6.0/docs/source/index.rst
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      648 2021-05-22 09:10:30.000000 pyreports-1.6.0/docs/source/install.rst
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     6139 2023-07-14 09:39:08.000000 pyreports-1.6.0/docs/source/managers.rst
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      201 2021-05-22 09:10:30.000000 pyreports-1.6.0/docs/source/package.rst
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      855 2022-08-04 10:18:33.000000 pyreports-1.6.0/docs/source/pyreports.rst
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     7906 2023-07-14 09:39:08.000000 pyreports-1.6.0/docs/source/report.rst
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    15086 2021-05-26 12:03:02.000000 pyreports-1.6.0/favicon.ico
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    19453 2022-09-27 09:45:00.000000 pyreports-1.6.0/index.html
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1359 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyproject.toml
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.781167 pyreports-1.6.0/pyreports/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1279 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyreports/__init__.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     9067 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyreports/cli.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    18933 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyreports/core.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     5068 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyreports/datatools.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1145 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyreports/exception.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)    20849 2023-07-14 09:39:08.000000 pyreports-1.6.0/pyreports/io.py
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.782167 pyreports-1.6.0/pyreports.egg-info/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     9612 2023-07-14 09:43:06.000000 pyreports-1.6.0/pyreports.egg-info/PKG-INFO
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1182 2023-07-14 09:43:06.000000 pyreports-1.6.0/pyreports.egg-info/SOURCES.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        1 2023-07-14 09:43:06.000000 pyreports-1.6.0/pyreports.egg-info/dependency_links.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       47 2023-07-14 09:43:06.000000 pyreports-1.6.0/pyreports.egg-info/entry_points.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       88 2023-07-14 09:43:06.000000 pyreports-1.6.0/pyreports.egg-info/requires.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       10 2023-07-14 09:43:06.000000 pyreports-1.6.0/pyreports.egg-info/top_level.txt
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)       38 2023-07-14 09:43:06.784167 pyreports-1.6.0/setup.cfg
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     1395 2023-07-14 09:39:08.000000 pyreports-1.6.0/setup.py
-drwxr-xr-x   0 matteo.guadrini  (1000) matteo.guadrini  (1000)        0 2023-07-14 09:43:06.783167 pyreports-1.6.0/tests/
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)      882 2022-04-15 12:42:39.000000 pyreports-1.6.0/tests/__init__.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8770 2023-07-14 09:39:08.000000 pyreports-1.6.0/tests/test_core.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     2390 2023-07-14 09:39:08.000000 pyreports-1.6.0/tests/test_data.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     6003 2022-04-15 12:42:39.000000 pyreports-1.6.0/tests/test_db.py
--rw-r--r--   0 matteo.guadrini  (1000) matteo.guadrini  (1000)     8192 2022-06-27 09:04:05.000000 pyreports-1.6.0/tests/test_file.py
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.021237 pyreports-1.7.0/
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.007237 pyreports-1.7.0/.circleci/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      547 2024-04-19 08:12:21.000000 pyreports-1.7.0/.circleci/config.yml
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.007237 pyreports-1.7.0/.github/
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.008237 pyreports-1.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      310 2021-05-22 09:10:30.000000 pyreports-1.7.0/.github/ISSUE_TEMPLATE/reports-enhancement.md
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      350 2021-05-22 09:10:30.000000 pyreports-1.7.0/.github/ISSUE_TEMPLATE/reports-issue.md
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      330 2020-09-16 09:59:48.000000 pyreports-1.7.0/.github/PULL_REQUEST_TEMPLATE.md
+-rwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)     3272 2021-05-01 12:43:38.000000 pyreports-1.7.0/.gitignore
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     1034 2024-04-19 08:12:21.000000 pyreports-1.7.0/.readthedocs.yaml
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     3932 2024-04-19 08:12:21.000000 pyreports-1.7.0/CHANGES.md
+-rw-rw-r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     2503 2019-10-29 13:39:34.000000 pyreports-1.7.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     4049 2019-10-28 14:57:18.000000 pyreports-1.7.0/CONTRIBUTING.md
+-rwxrwxr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)    34916 2019-10-26 09:26:26.000000 pyreports-1.7.0/LICENSE.md
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       22 2023-07-14 09:39:08.000000 pyreports-1.7.0/MANIFEST.in
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     9787 2024-04-19 08:15:03.020237 pyreports-1.7.0/PKG-INFO
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     8513 2022-09-27 09:45:00.000000 pyreports-1.7.0/README.md
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.008237 pyreports-1.7.0/assets/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     8196 2022-04-15 12:42:38.000000 pyreports-1.7.0/assets/.DS_Store
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.009237 pyreports-1.7.0/assets/css/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     6148 2022-04-15 12:42:38.000000 pyreports-1.7.0/assets/css/.DS_Store
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    12830 2021-05-26 12:03:02.000000 pyreports-1.7.0/assets/css/theme-1.css
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.009237 pyreports-1.7.0/assets/js/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     6148 2022-04-15 12:42:38.000000 pyreports-1.7.0/assets/js/.DS_Store
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      882 2021-05-26 12:03:02.000000 pyreports-1.7.0/assets/js/main.js
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.010237 pyreports-1.7.0/docs/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      638 2021-05-08 08:55:41.000000 pyreports-1.7.0/docs/Makefile
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      764 2021-05-08 08:55:41.000000 pyreports-1.7.0/docs/make.bat
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       72 2024-04-19 08:12:21.000000 pyreports-1.7.0/docs/requirements.txt
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.013237 pyreports-1.7.0/docs/source/
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.013237 pyreports-1.7.0/docs/source/_static/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    14659 2021-05-26 10:37:38.000000 pyreports-1.7.0/docs/source/_static/pyreports.svg
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     2112 2024-04-19 08:12:21.000000 pyreports-1.7.0/docs/source/conf.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     7667 2024-04-19 08:12:21.000000 pyreports-1.7.0/docs/source/datatools.rst
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.014237 pyreports-1.7.0/docs/source/dev/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     8840 2023-07-14 09:39:08.000000 pyreports-1.7.0/docs/source/dev/cli.rst
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     5896 2021-05-22 09:10:30.000000 pyreports-1.7.0/docs/source/dev/core.rst
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     3801 2023-07-14 09:39:08.000000 pyreports-1.7.0/docs/source/dev/io.rst
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    11452 2024-04-19 08:12:21.000000 pyreports-1.7.0/docs/source/example.rst
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     8402 2021-05-22 09:10:30.000000 pyreports-1.7.0/docs/source/executors.rst
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     2066 2022-08-04 10:18:33.000000 pyreports-1.7.0/docs/source/index.rst
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      648 2021-05-22 09:10:30.000000 pyreports-1.7.0/docs/source/install.rst
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     5996 2024-04-19 08:12:21.000000 pyreports-1.7.0/docs/source/managers.rst
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      201 2021-05-22 09:10:30.000000 pyreports-1.7.0/docs/source/package.rst
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      855 2022-08-04 10:18:33.000000 pyreports-1.7.0/docs/source/pyreports.rst
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     7906 2023-07-14 09:39:08.000000 pyreports-1.7.0/docs/source/report.rst
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    15086 2021-05-26 12:03:02.000000 pyreports-1.7.0/favicon.ico
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    19489 2024-04-19 08:12:21.000000 pyreports-1.7.0/index.html
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     1321 2024-04-19 08:12:21.000000 pyreports-1.7.0/pyproject.toml
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.016237 pyreports-1.7.0/pyreports/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     1616 2024-04-19 08:12:21.000000 pyreports-1.7.0/pyreports/__init__.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     9225 2024-04-19 08:12:21.000000 pyreports-1.7.0/pyreports/cli.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    19316 2024-04-19 08:12:21.000000 pyreports-1.7.0/pyreports/core.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     8595 2024-04-19 08:12:21.000000 pyreports-1.7.0/pyreports/datatools.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     1196 2024-04-19 08:12:21.000000 pyreports-1.7.0/pyreports/exception.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    20617 2024-04-19 08:12:21.000000 pyreports-1.7.0/pyreports/io.py
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.019237 pyreports-1.7.0/pyreports.egg-info/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     9787 2024-04-19 08:15:02.000000 pyreports-1.7.0/pyreports.egg-info/PKG-INFO
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     1200 2024-04-19 08:15:02.000000 pyreports-1.7.0/pyreports.egg-info/SOURCES.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)        1 2024-04-19 08:15:02.000000 pyreports-1.7.0/pyreports.egg-info/dependency_links.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       47 2024-04-19 08:15:02.000000 pyreports-1.7.0/pyreports.egg-info/entry_points.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       80 2024-04-19 08:15:02.000000 pyreports-1.7.0/pyreports.egg-info/requires.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       10 2024-04-19 08:15:02.000000 pyreports-1.7.0/pyreports.egg-info/top_level.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       38 2024-04-19 08:15:03.021237 pyreports-1.7.0/setup.cfg
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     1374 2024-04-19 08:12:21.000000 pyreports-1.7.0/setup.py
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-19 08:15:03.019237 pyreports-1.7.0/tests/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      882 2022-04-15 12:42:39.000000 pyreports-1.7.0/tests/__init__.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     8770 2023-07-14 09:39:08.000000 pyreports-1.7.0/tests/test_core.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     7406 2024-04-19 08:12:21.000000 pyreports-1.7.0/tests/test_data.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     5092 2024-04-19 08:12:21.000000 pyreports-1.7.0/tests/test_db.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     8192 2022-06-27 09:04:05.000000 pyreports-1.7.0/tests/test_file.py
```

### Comparing `pyreports-1.6.0/.circleci/config.yml` & `pyreports-1.7.0/.circleci/config.yml`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,15 @@
   build-and-test:
     docker:
       - image: circleci/python
     steps:
       - checkout
       - run: sudo apt update && sudo apt install -y freetds-dev libssl-dev python-dev freetds-bin
       - run: sudo pip install --upgrade pip
-      - run: sudo pip install cython
-      - run: sudo pip install pymssql
+      - run: sudo pip install "Cython<3"
       - run: sudo pip install numpy
       - run: sudo pip install pandas
       - run: sudo python setup.py install
       - run: sudo chmod -R 777 /tmp
       - run: sudo python -m unittest discover tests
 
 workflows:
```

### Comparing `pyreports-1.6.0/.gitignore` & `pyreports-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/CODE_OF_CONDUCT.md` & `pyreports-1.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/CONTRIBUTING.md` & `pyreports-1.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/LICENSE.md` & `pyreports-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/PKG-INFO` & `pyreports-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: pyreports
-Version: 1.6.0
+Version: 1.7.0
 Summary: pyreports is a python library that allows you to create complex report from various sources.
 Home-page: https://github.com/MatteoGuadrini/pyreports
 Author: Matteo Guadrini
 Author-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 Maintainer: Matteo Guadrini
 Maintainer-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 License: GNU General Public License v3.0
 Project-URL: homepage, https://github.com/MatteoGuadrini/pyreports'
 Project-URL: documentation, https://pyreports.readthedocs.io/en/latest/
-Project-URL: repository, https://github.com/MatteoGuadrini/pyreports/pyreports.git
+Project-URL: repository, https://github.com/MatteoGuadrini/pyreports.git
 Project-URL: changelog, https://github.com/MatteoGuadrini/pyreports/blob/master/CHANGES.md
 Keywords: pyreports,reports,report,csv,yaml,export,excel,database,ldap,dataset,file,executor,book
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: ldap3
+Requires-Dist: mysql-connector-python
+Requires-Dist: psycopg2-binary
+Requires-Dist: tablib
+Requires-Dist: tablib[all]
+Requires-Dist: nosqlapi
+Requires-Dist: pyyaml
 
 # pyreports
 
 <img src="https://pyreports.readthedocs.io/en/latest/_static/pyreports.svg" alt="pyreports" title="pyreports" width="300" height="300" />
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/2bad30d308414c83836f22f012c98649)](https://www.codacy.com/gh/MatteoGuadrini/pyreports/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=MatteoGuadrini/pyreports&amp;utm_campaign=Badge_Grade)
 [![CircleCI](https://circleci.com/gh/MatteoGuadrini/pyreports.svg?style=svg)](https://circleci.com/gh/MatteoGuadrini/pyreports)
```

### Comparing `pyreports-1.6.0/README.md` & `pyreports-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/assets/.DS_Store` & `pyreports-1.7.0/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/assets/css/.DS_Store` & `pyreports-1.7.0/assets/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/assets/css/theme-1.css` & `pyreports-1.7.0/assets/css/theme-1.css`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/assets/js/.DS_Store` & `pyreports-1.7.0/assets/js/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/assets/js/main.js` & `pyreports-1.7.0/assets/js/main.js`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/docs/Makefile` & `pyreports-1.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/docs/make.bat` & `pyreports-1.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/docs/source/_static/pyreports.svg` & `pyreports-1.7.0/docs/source/_static/pyreports.svg`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/docs/source/conf.py` & `pyreports-1.7.0/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,36 +11,35 @@
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 import os
 import sys
-sys.path.insert(0, os.path.abspath('../..'))
 
-import __info__
+sys.path.insert(0, os.path.abspath("../.."))
 
 # -- Project information -----------------------------------------------------
 
-project = 'pyreports'
-copyright = '2021, Matteo Guadrini'
-author = __info__.__author__
+project = "pyreports"
+copyright = "2024, Matteo Guadrini"
+author = "Matteo Guadrini"
 
 # The full version, including alpha/beta/rc tags
-release = __info__.__version__
+release = "1.7.0"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest']
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.doctest"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = []
 
 # -- Options for HTML output -------------------------------------------------
@@ -49,15 +48,13 @@
 # a list of builtin themes.
 #
 html_theme = "sphinx_rtd_theme"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
-html_theme_options = {
-    'logo_only': False
-}
+html_theme_options = {"logo_only": False}
 html_logo = "_static/pyreports.svg"
 
-master_doc = 'index'
+master_doc = "index"
```

### Comparing `pyreports-1.6.0/docs/source/dev/cli.rst` & `pyreports-1.7.0/docs/source/dev/cli.rst`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/docs/source/dev/core.rst` & `pyreports-1.7.0/docs/source/dev/core.rst`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/docs/source/dev/io.rst` & `pyreports-1.7.0/docs/source/dev/io.rst`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/docs/source/example.rst` & `pyreports-1.7.0/docs/source/example.rst`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     import pyreports
 
     # INPUT
 
     # Config Unix application file: this is a FileManager object
     config_file = pyreports.manager('yaml', '/home/myapp.yml')
     # Console admin: this is a DatabaseManager object
-    mydb = pyreports.manager('mssql', server='mssql1.local', database='admins', user='sa', password='sa0000')
+    mydb = pyreports.manager('mysql', server='mysql1.local', database='admins', user='sa', password='sa0000')
     # Get data
     admin_app = config_file.read()                  # return Dataset object: three column (name, shell, login)
     mydb.execute('SELECT * FROM console_admins')
     admins = mydb.fetchall()                        # return Dataset object: three column (name, shell, login)
 
     # PROCESS
```

### Comparing `pyreports-1.6.0/docs/source/executors.rst` & `pyreports-1.7.0/docs/source/executors.rst`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/docs/source/index.rst` & `pyreports-1.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/docs/source/install.rst` & `pyreports-1.7.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/docs/source/managers.rst` & `pyreports-1.7.0/docs/source/managers.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 Type of managers
 ****************
 
 Each type of manager is managed by micro types; Below is the complete list:
 
 #. Database
     #. sqlite (SQLite)
-    #. mssql (Microsoft SQL)
     #. mysql (MySQL or MariaDB)
     #. postgresql (PostgreSQL or EnterpriseDB)
 #. File
     #. file (standard text file)
     #. log (log file)
     #. csv (Comma Separated Value file)
     #. json (JSON file)
@@ -37,15 +36,14 @@
 
 .. code-block:: python
 
     import pyreports
 
     # DatabaseManager object
     sqlite_db = pyreports.manager('sqlite', database='/tmp/mydb.db')
-    mssql_db = pyreports.manager('mssql', server='mssql1.local', database='test', user='dba', password='dba0000')
     mysql_db = pyreports.manager('mysql', host='mysql1.local', database='test', user='dba', password='dba0000')
     postgresql_db = pyreports.manager('postgresql', host='postgresql1.local', database='test', user='dba', password='dba0000')
 
     # FileManager object
     file = pyreports.manager('file', '/tmp/text.txt')
     log = pyreports.manager('log', '/tmp/log.log')
     csv = pyreports.manager('csv', '/tmp/csv.csv')
```

### Comparing `pyreports-1.6.0/docs/source/pyreports.rst` & `pyreports-1.7.0/docs/source/pyreports.rst`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/docs/source/report.rst` & `pyreports-1.7.0/docs/source/report.rst`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/favicon.ico` & `pyreports-1.7.0/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/index.html` & `pyreports-1.7.0/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -241,32 +241,32 @@
             <div class="block">
                 <h3 class="sub-title text-center">Shell CLI</h3>
                 <p>pyreports has a command line interface which takes a configuration file in <b>YAML</b> format as an argument.</p>
                 <div class="code-block">
                     <pre><code class="language-shell">
 $ cat car.yml
 reports:
-- report:
-  title: 'Red ford machine'
-  input:
-    manager: 'mysql'
-    source:
-    # Connection parameters of my mysql database
-      host: 'mysql1.local'
-      database: 'cars'
-      user: 'admin'
-      password: 'dba0000'
-    params:
-      query: 'SELECT * FROM cars WHERE brand = %s AND color = %s'
-      params: ['ford', 'red']
-  # Filter km
-  filters: [40000, 45000]
-  output:
-    manager: 'csv'
-    filename: '/tmp/car_csv.csv'
+  - report:
+    title: 'Red ford machine'
+    input:
+      manager: 'mysql'
+      source:
+      # Connection parameters of my mysql database
+        host: 'mysql1.local'
+        database: 'cars'
+        user: 'admin'
+        password: 'dba0000'
+      params:
+        query: 'SELECT * FROM cars WHERE brand = %s AND color = %s'
+        params: ['ford', 'red']
+    # Filter km
+    filters: [40000, 45000]
+    output:
+      manager: 'csv'
+      filename: '/tmp/car_csv.csv'
 
 $ report car.yaml
                     </code></pre>
                 </div><!--//code-block-->
             </div><!--//block Shell CLI-->
 
             <div class="block">
```

#### html2text {}

```diff
@@ -102,32 +102,32 @@
 
 ******** SShheellll CCLLII ********
 pyreports has a command line interface which takes a configuration file in YYAAMMLL
 format as an argument.
 
 $ cat car.yml
 reports:
-- report:
-  title: 'Red ford machine'
-  input:
-    manager: 'mysql'
-    source:
-    # Connection parameters of my mysql database
-      host: 'mysql1.local'
-      database: 'cars'
-      user: 'admin'
-      password: 'dba0000'
-    params:
-      query: 'SELECT * FROM cars WHERE brand = %s AND color = %s'
-      params: ['ford', 'red']
-  # Filter km
-  filters: [40000, 45000]
-  output:
-    manager: 'csv'
-    filename: '/tmp/car_csv.csv'
+  - report:
+    title: 'Red ford machine'
+    input:
+      manager: 'mysql'
+      source:
+      # Connection parameters of my mysql database
+        host: 'mysql1.local'
+        database: 'cars'
+        user: 'admin'
+        password: 'dba0000'
+      params:
+        query: 'SELECT * FROM cars WHERE brand = %s AND color = %s'
+        params: ['ford', 'red']
+    # Filter km
+    filters: [40000, 45000]
+    output:
+      manager: 'csv'
+      filename: '/tmp/car_csv.csv'
 
 $ report car.yaml
 
 ******** FFuullll DDooccuummeennttaattiioonn ********
 The complete documentation is much more comprehensive and can be found by
 clicking the button below.
 _M_o_r_e_ _o_n_ _R_e_a_d_T_h_e_D_o_c_s
```

### Comparing `pyreports-1.6.0/pyproject.toml` & `pyreports-1.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["setuptools", "setuptools_scm[toml]", "wheel", "cython"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyreports"
-version = "1.6.0"
+version = "1.7.0"
 readme = "README.md"
-license = {text = "GNU General Public License v3.0"}
+license = { text = "GNU General Public License v3.0" }
 keywords = ['pyreports', 'reports', 'report', 'csv', 'yaml', 'export',
-            'excel', 'database', 'ldap', 'dataset', 'file', 'executor', 'book']
+    'excel', 'database', 'ldap', 'dataset', 'file', 'executor', 'book']
 authors = [{ name = "Matteo Guadrini", email = "matteo.guadrini@hotmail.it" }]
 maintainers = [
     { name = "Matteo Guadrini", email = "matteo.guadrini@hotmail.it" },
 ]
 description = "pyreports is a python library that allows you to create complex report from various sources."
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
-dependencies = ['ldap3', 'pymssql', 'mysql-connector-python',
-                'psycopg2-binary', 'tablib', 'tablib[all]', 'nosqlapi', 'pyyaml']
+dependencies = ['ldap3', 'mysql-connector-python',
+    'psycopg2-binary', 'tablib', 'tablib[all]', 'nosqlapi', 'pyyaml']
 
 [project.scripts]
 reports = "pyreports.cli:main"
 
 [project.urls]
 homepage = "https://github.com/MatteoGuadrini/pyreports'"
 documentation = "https://pyreports.readthedocs.io/en/latest/"
-repository = "https://github.com/MatteoGuadrini/pyreports/pyreports.git"
-changelog = "https://github.com/MatteoGuadrini/pyreports/blob/master/CHANGES.md"
+repository = "https://github.com/MatteoGuadrini/pyreports.git"
+changelog = "https://github.com/MatteoGuadrini/pyreports/blob/master/CHANGES.md"
```

### Comparing `pyreports-1.6.0/pyreports/cli.py` & `pyreports-1.7.0/pyreports/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # cli -- pyreports
 #
-#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2024 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -24,62 +24,68 @@
 
 # region imports
 import sys
 import tablib
 import yaml
 import argparse
 import pyreports
-
-# endregion
-
-# region globals
-__version__ = '1.5.1'
+from pyreports import __version__
 
 
 # endregion
 
+
 # region functions
 def get_args():
     """Get command-line arguments"""
 
     parser = argparse.ArgumentParser(
-        description='pyreports command line interface (CLI)',
+        description="pyreports command line interface (CLI)",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        epilog='Full docs here: https://pyreports.readthedocs.io/en/latest/dev/cli.html'
+        epilog="Full docs here: https://pyreports.readthedocs.io/en/latest/dev/cli.html",
     )
 
-    parser.add_argument('config',
-                        metavar='CONFIG_FILE',
-                        default=sys.stdin,
-                        type=argparse.FileType('rt', encoding="utf-8"),
-                        help='YAML configuration file')
-    parser.add_argument('-e', '--exclude',
-                        help='Excluded title report list',
-                        nargs=argparse.ZERO_OR_MORE,
-                        default=[],
-                        metavar='TITLE')
-    parser.add_argument('-v', '--verbose', help='Enable verbose mode', action='store_true')
-    parser.add_argument('-V', '--version', help='Print version', action='version', version=__version__)
+    parser.add_argument(
+        "config",
+        metavar="CONFIG_FILE",
+        default=sys.stdin,
+        type=argparse.FileType("rt", encoding="utf-8"),
+        help="YAML configuration file",
+    )
+    parser.add_argument(
+        "-e",
+        "--exclude",
+        help="Excluded title report list",
+        nargs=argparse.ZERO_OR_MORE,
+        default=[],
+        metavar="TITLE",
+    )
+    parser.add_argument(
+        "-v", "--verbose", help="Enable verbose mode", action="store_true"
+    )
+    parser.add_argument(
+        "-V", "--version", help="Print version", action="version", version=__version__
+    )
 
     args = parser.parse_args()
     filename = args.config.name
 
     # Check if file is a YAML file
     try:
         args.config = load_config(args.config)
     except yaml.YAMLError as err:
-        parser.error(f'file {filename} is not a valid YAML file: \n{err}')
+        parser.error(f"file {filename} is not a valid YAML file: \n{err}")
 
     # Validate config file
     try:
         validate_config(args.config)
     except yaml.YAMLError as err:
         parser.error(str(err))
 
-    print_verbose(f'parsed YAML file {filename}', verbose=args.verbose)
+    print_verbose(f"parsed YAML file {filename}", verbose=args.verbose)
 
     return args
 
 
 def load_config(yaml_file):
     """Load configuration file
 
@@ -93,41 +99,47 @@
 def validate_config(config):
     """Validate config object
 
     :param config: YAML config object
     :return: None
     """
     try:
-        reports = config['reports']
+        reports = config["reports"]
         if reports is None or not isinstance(reports, list):
             raise yaml.YAMLError('"reports" section have not "report" list sections')
-        datas = all([bool(report.get('report').get('input')) for report in reports])
+        datas = all([bool(report.get("report").get("input")) for report in reports])
         if not datas:
             raise yaml.YAMLError(
                 'one of "report" section does not have "input" section'
             )
     except KeyError as err:
         raise yaml.YAMLError(f'there is no "{err}" section')
     except AttributeError:
-        raise yaml.YAMLError('correctly indents the "report" section or "report" section not exists')
+        raise yaml.YAMLError(
+            'correctly indents the "report" section or "report" section not exists'
+        )
 
 
 def make_manager(input_config):
     """Make Manager object
 
     :param input_config: file, sql or nosql report configuration
     :return: manager
     """
 
-    type_ = input_config.get('manager')
+    type_ = input_config.get("manager")
 
     if type_ in pyreports.io.FILETYPE:
-        manager = pyreports.manager(input_config.get('manager'), input_config.get('filename', ()))
+        manager = pyreports.manager(
+            input_config.get("manager"), input_config.get("filename", ())
+        )
     else:
-        manager = pyreports.manager(input_config.get('manager'), **input_config.get('source', {}))
+        manager = pyreports.manager(
+            input_config.get("manager"), **input_config.get("source", {})
+        )
 
     return manager
 
 
 def get_data(manager, params=None):
     """Get Dataset from source
 
@@ -135,37 +147,37 @@
     :param params: parameter used into call of method in Manager object
     :return: Dataset
     """
     if params is None:
         params = ()
     data = None
     # FileManager
-    if manager.type == 'file':
+    if manager.type == "file":
         if params and isinstance(params, (list, tuple)):
             data = manager.read(*params)
         elif params and isinstance(params, dict):
             data = manager.read(**params)
         else:
             data = manager.read()
     # DatabaseManager
-    elif manager.type == 'sql':
+    elif manager.type == "sql":
         if params and isinstance(params, (list, tuple)):
             manager.execute(*params)
             data = manager.fetchall()
         elif params and isinstance(params, dict):
             manager.execute(**params)
             data = manager.fetchall()
     # LdapManager
-    elif manager.type == 'ldap':
+    elif manager.type == "ldap":
         if params and isinstance(params, (list, tuple)):
             data = manager.query(*params)
         elif params and isinstance(params, dict):
             data = manager.query(**params)
     # NosqlManager
-    elif manager.type == 'nosql':
+    elif manager.type == "nosql":
         if params and isinstance(params, (list, tuple)):
             data = manager.find(*params)
         elif params and isinstance(params, dict):
             data = manager.find(**params)
 
     return data
 
@@ -174,94 +186,107 @@
     """Print messages if verbose is True
 
     :param messages: some string messages
     :param verbose: enable or disable verbosity
     :return: None
     """
     if verbose:
-        print('info:', *messages)
+        print("info:", *messages)
 
 
 def main():
     """Main logic"""
 
     # Get command line args
     args = get_args()
     # Take reports
     config = args.config
-    reports = config.get('reports', ())
+    reports = config.get("reports", ())
 
-    print_verbose(f'found {len(config.get("reports", ()))} report(s)',
-                  verbose=args.verbose)
+    print_verbose(
+        f'found {len(config.get("reports", ()))} report(s)', verbose=args.verbose
+    )
 
     # Build the data and report
     for report in reports:
         # Check if report isn't in excluded list
-        if args.exclude and report.get('report').get('title') in args.exclude:
-            print_verbose(f'exclude report "{report.get("report").get("title")}"',
-                          verbose=args.verbose)
+        if args.exclude and report.get("report").get("title") in args.exclude:
+            print_verbose(
+                f'exclude report "{report.get("report").get("title")}"',
+                verbose=args.verbose,
+            )
             continue
         # Make a manager object
-        input_ = report.get('report').get('input')
-        print_verbose(f'make an input manager of type {input_.get("manager")}',
-                      verbose=args.verbose)
+        input_ = report.get("report").get("input")
+        print_verbose(
+            f'make an input manager of type {input_.get("manager")}',
+            verbose=args.verbose,
+        )
         manager = make_manager(input_)
         # Get data
-        print_verbose(f'get data from manager {manager}', verbose=args.verbose)
+        print_verbose(f"get data from manager {manager}", verbose=args.verbose)
         try:
             # Make a report object
-            data = get_data(manager, input_.get('params'))
-            if 'map' in report.get('report'):
-                exec(report.get('report').get('map'))
-            map_func = globals().get('map_func')
+            data = get_data(manager, input_.get("params"))
+            if "map" in report.get("report"):
+                exec(report.get("report").get("map"))
+            map_func = globals().get("map_func")
             report_ = pyreports.Report(
                 input_data=data,
-                title=report.get('report').get('title'),
-                filters=report.get('report').get('filters'),
+                title=report.get("report").get("title"),
+                filters=report.get("report").get("filters"),
                 map_func=map_func,
-                negation=report.get('report').get('negation', False),
-                column=report.get('report').get('column'),
-                count=report.get('report').get('count', False),
-                output=make_manager(report.get('report').get('output')) if 'output' in report.get('report') else None
+                negation=report.get("report").get("negation", False),
+                column=report.get("report").get("column"),
+                count=report.get("report").get("count", False),
+                output=make_manager(report.get("report").get("output"))
+                if "output" in report.get("report")
+                else None,
             )
             print_verbose(f'created report "{report_.title}"', verbose=args.verbose)
         except Exception as err:
             pyreports.Report(tablib.Dataset())
-            exit(f'error: {err}')
+            exit(f"error: {err}")
         # Check output
         if report_.output:
             # Check if export or send report
-            if report.get('report').get('mail'):
-                print_verbose(f'send report to {report.get("report").get("mail").get("to")}', verbose=args.verbose)
-                mail_settings = report.get('report').get('mail')
+            if report.get("report").get("mail"):
+                print_verbose(
+                    f'send report to {report.get("report").get("mail").get("to")}',
+                    verbose=args.verbose,
+                )
+                mail_settings = report.get("report").get("mail")
                 report_.send(
-                    server=mail_settings.get('server'),
-                    _from=mail_settings.get('from'),
-                    to=mail_settings.get('to'),
-                    cc=mail_settings.get('cc'),
-                    bcc=mail_settings.get('bcc'),
-                    subject=mail_settings.get('subject'),
-                    body=mail_settings.get('body'),
-                    auth=tuple(mail_settings.get('auth')) if 'auth' in mail_settings else None,
-                    _ssl=bool(mail_settings.get('ssl')),
-                    headers=mail_settings.get('headers')
+                    server=mail_settings.get("server"),
+                    _from=mail_settings.get("from"),
+                    to=mail_settings.get("to"),
+                    cc=mail_settings.get("cc"),
+                    bcc=mail_settings.get("bcc"),
+                    subject=mail_settings.get("subject"),
+                    body=mail_settings.get("body"),
+                    auth=tuple(mail_settings.get("auth"))
+                    if "auth" in mail_settings
+                    else None,
+                    _ssl=bool(mail_settings.get("ssl")),
+                    headers=mail_settings.get("headers"),
                 )
             else:
-                print_verbose(f'export report to {report_.output}',
-                              verbose=args.verbose)
+                print_verbose(
+                    f"export report to {report_.output}", verbose=args.verbose
+                )
                 report_.export()
         else:
             # Print report in stdout
-            print_verbose('print report to stdout', verbose=args.verbose)
-            title = report.get('report').get('title')
+            print_verbose("print report to stdout", verbose=args.verbose)
+            title = report.get("report").get("title")
             report_.exec()
             print(f"{title}\n{'=' * len(title)}\n")
             print(report_)
 
 
 # endregion
 
 # region main
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
 
 # endregion
```

### Comparing `pyreports-1.6.0/pyreports/core.py` & `pyreports-1.7.0/pyreports/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # core -- pyreports
 #
-#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2024 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -27,22 +27,24 @@
 import ssl
 import tablib
 import smtplib
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 from email import encoders
 from email.mime.base import MIMEBase
+from .datatools import DataAdapters, DataPrinters
 from .io import Manager, WRITABLE_MANAGER
 from .exception import ReportManagerError, ReportDataError, ExecutorError
 
 
 # endregion
 
 # region Classes
 
+
 class Executor:
     """Executor receives, processes, transforms and writes data"""
 
     def __init__(self, data, header=None):
         """Create Executor object
 
         :param data: everything type of data
@@ -246,56 +248,57 @@
         """Clone Executor object
 
         :return: executor
         """
         return Executor(self.origin, header=self.origin.headers)
 
 
-class Report:
+class Report(DataAdapters, DataPrinters):
     """Report represents the workflow for generating a report"""
 
-    def __init__(self,
-                 input_data: tablib.Dataset,
-                 title=None,
-                 filters=None,
-                 map_func=None,
-                 negation=False,
-                 column=None,
-                 count=False,
-                 output: Manager = None):
+    def __init__(
+        self,
+        input_data: tablib.Dataset,
+        title=None,
+        filters=None,
+        map_func=None,
+        negation=False,
+        column=None,
+        count=False,
+        output: Manager = None,
+    ):
         """Create Report object
 
         :param input_data: Dataset object
         :param title: title of Report object
         :param filters: list or function for filter data
         :param map_func: function for modifying data
         :param negation: enable negation for filters or map_func
         :param column: select column name or index
         :param count: count rows
         :param output: Manager object
         """
         # Discard all objects that are not Datasets
-        if isinstance(input_data, tablib.Dataset):
-            self.data = input_data
-        else:
-            raise ReportDataError('Only Dataset object is allowed for input')
+        DataAdapters.__init__(self, input_data=input_data)
         # Set other arguments
         self.title = title
         self.filter = filters
         self.map = map_func
         self.negation = negation
         self.column = column
         self.count = bool(count)
         if isinstance(output, Manager) or output is None:
             if output:
                 if output.__class__.__name__ not in WRITABLE_MANAGER:
-                    raise ReportManagerError(f'Only {WRITABLE_MANAGER} object is allowed for output')
+                    raise ReportManagerError(
+                        f"Only {WRITABLE_MANAGER} object is allowed for output"
+                    )
             self.output = output
         else:
-            raise ReportManagerError('Only Manager object is allowed for output')
+            raise ReportManagerError("Only Manager object is allowed for output")
         # Data for report
         self.report = None
 
     def __repr__(self):
         """Representation of Report object
 
         :return: string
@@ -342,15 +345,15 @@
 
     def _print_data(self):
         """Print data and count
 
         :return: data and count
         """
         if self.count:
-            out = f'{self.report}\nrows: {int(self.count)}'
+            out = f"{self.report}\nrows: {int(self.count)}"
             return out
         else:
             return self.report
 
     def exec(self):
         """Create Executor object to apply filters and map function to input data
 
@@ -376,42 +379,53 @@
         """Process and save data on output
 
         :return: if count is True, return row count
         """
         # Process data before export
         self.exec()
         if self.output is not None:
-            if self.output.type == 'file':
+            if self.output.type == "file":
                 self.output.write(self.report)
-            elif self.output.type == 'sql':
+            elif self.output.type == "sql":
                 if not self.report.headers:
                     raise ReportDataError("Dataset object doesn't have a header")
-                table_name = self.title.replace(' ', '_').lower()
-                fields = ','.join([
-                    f'{field} VARCHAR(255)'
-                    for field in self.report.headers
-                ])
+                table_name = self.title.replace(" ", "_").lower()
+                fields = ",".join(
+                    [f"{field} VARCHAR(255)" for field in self.report.headers]
+                )
                 # Create table with header
                 self.output.execute(
                     f"CREATE TABLE IF NOT EXISTS {table_name} ({fields});"
                 )
                 # Insert data into table
-                table_header = ','.join(field for field in self.report.headers)
+                table_header = ",".join(field for field in self.report.headers)
                 for row in self.report:
                     row_table = [f"'{element}'" for element in row]
                     self.output.execute(
                         f"INSERT INTO {table_name} "
                         f"({table_header}) "
                         f"VALUES ({','.join(element for element in row_table)});"
                     )
                 self.output.commit()
         else:
             print(self)
 
-    def send(self, server, _from, to, cc=None, bcc=None, subject=None, body='', auth=None, _ssl=True, headers=None):
+    def send(
+        self,
+        server,
+        _from,
+        to,
+        cc=None,
+        bcc=None,
+        subject=None,
+        body="",
+        auth=None,
+        _ssl=True,
+        headers=None,
+    ):
         """Send saved report to email
 
         :param server: server SMTP
         :param _from: email address 'from:'
         :param to: email address 'to:'
         :param cc: email address 'cc:'
         :param bcc: email address 'bcc:'
@@ -419,15 +433,17 @@
         :param body: email body
         :param auth: authorization tuple "(user, password)"
         :param _ssl: boolean, if True port is 465 else 25
         :param headers: more header value "(header_name, key, value)"
         :return: None
         """
         if not self.output:
-            raise ReportDataError('if you want send a mail with a report in attachment, must be specified output')
+            raise ReportDataError(
+                "if you want send a mail with a report in attachment, must be specified output"
+            )
 
         # Prepare mail header
         message = MIMEMultipart("alternative")
         message["Subject"] = self.title if not subject else subject
         message["From"] = _from
         message["To"] = to
         if cc:
@@ -437,43 +453,51 @@
         if headers:
             if all([isinstance(header, (tuple, list)) for header in headers]):
                 for header in headers:
                     message.add_header(*header)
             elif isinstance(headers, (tuple, list)):
                 message.add_header(*headers)
             else:
-                raise ValueError('headers must be tuple or List[tuple]')
+                raise ValueError("headers must be tuple or List[tuple]")
 
         # Prepare body
         part = MIMEText(body, "html")
         message.attach(part)
 
         # Prepare attachment
         self.export()
         attach_file_name = self.output.data.file
-        attach_file = open(attach_file_name, 'rb')
-        payload = MIMEBase('application', 'octate-stream')
+        attach_file = open(attach_file_name, "rb")
+        payload = MIMEBase("application", "octate-stream")
         payload.set_payload(attach_file.read())
         encoders.encode_base64(payload)
-        payload.add_header('Content-Disposition', 'attachment', filename=os.path.basename(attach_file_name))
+        payload.add_header(
+            "Content-Disposition",
+            "attachment",
+            filename=os.path.basename(attach_file_name),
+        )
         message.attach(payload)
 
         # Prepare SMTP connection
         if _ssl:
             port = smtplib.SMTP_SSL_PORT
             protocol = smtplib.SMTP_SSL
-            kwargs = {'context': ssl.create_default_context()}
+            kwargs = {"context": ssl.create_default_context()}
         else:
             port = smtplib.SMTP_PORT
             protocol = smtplib.SMTP
             kwargs = {}
         with protocol(server, port, **kwargs) as srv:
             if auth:
                 srv.login(*auth)
-            srv.sendmail(_from, [receiver for receiver in (to, cc, bcc) if receiver], message.as_string())
+            srv.sendmail(
+                _from,
+                [receiver for receiver in (to, cc, bcc) if receiver],
+                message.as_string(),
+            )
 
 
 class ReportBook:
     """ReportBook represent a collection of Report's object"""
 
     def __init__(self, reports=None, title=None):
         """Create a ReportBook object
@@ -491,15 +515,15 @@
     def __add__(self, other):
         """Add report object
 
         :param other: Report object
         :return: ReportBook
         """
         if not isinstance(other, ReportBook):
-            raise ReportDataError('you can only add ReportBook object')
+            raise ReportDataError("you can only add ReportBook object")
         self.reports.extend(other.reports)
         return self
 
     def __iter__(self):
         """Return report iterator
 
         :return: iterable object
@@ -514,17 +538,16 @@
         return len(self.reports)
 
     def __str__(self):
         """Pretty representation of ReportBook object
 
         :return: string
         """
-        output = f'ReportBook {self.title if self.title else None}\n'
-        output += '\n'.join('\t' + str(report.title)
-                            for report in self.reports)
+        output = f"ReportBook {self.title if self.title else None}\n"
+        output += "\n".join("\t" + str(report.title) for report in self.reports)
         return output
 
     def __repr__(self):
         """Representation of ReportBook object
 
         :return: string
         """
@@ -557,15 +580,15 @@
     def add(self, report: Report):
         """Add report object
 
         :param report: Report object
         :return: None
         """
         if not isinstance(report, Report):
-            raise ReportDataError('you can only add Report object')
+            raise ReportDataError("you can only add Report object")
         self.reports.append(report)
 
     def remove(self, index: int = None):
         """Remove Report object, last added or index specified
 
         :param index: report number to remove
         :return: None
@@ -584,21 +607,33 @@
         if output:
             # Prepare pyreports
             for report in self:
                 report.exec()
             # Prepare book for export
             book = tablib.Databook(tuple([report.report for report in self]))
             # Save Excel WorkBook
-            with open(output, 'wb') as f:
-                f.write(book.export('xlsx'))
+            with open(output, "wb") as f:
+                f.write(book.export("xlsx"))
         else:
             for report in self:
                 report.export()
 
-    def send(self, server, _from, to, cc=None, bcc=None, subject=None, body='', auth=None, _ssl=True, headers=None):
+    def send(
+        self,
+        server,
+        _from,
+        to,
+        cc=None,
+        bcc=None,
+        subject=None,
+        body="",
+        auth=None,
+        _ssl=True,
+        headers=None,
+    ):
         """Send saved report to email
 
         :param server: server SMTP
         :param _from: email address 'from:'
         :param to: email address 'to:'
         :param cc: email address 'cc:'
         :param bcc: email address 'bcc:'
@@ -606,11 +641,22 @@
         :param body: email body
         :param auth: authorization tuple "(user, password)"
         :param _ssl: boolean, if True port is 465 else 25
         :param headers: more header value "(header_name, key, value)"
         :return: None
         """
         for report in self:
-            report.send(server, _from, to, cc=cc, bcc=bcc, subject=subject, body=body, auth=auth,
-                        _ssl=_ssl, headers=headers)
+            report.send(
+                server,
+                _from,
+                to,
+                cc=cc,
+                bcc=bcc,
+                subject=subject,
+                body=body,
+                auth=auth,
+                _ssl=_ssl,
+                headers=headers,
+            )
+
 
 # endregion
```

### Comparing `pyreports-1.6.0/pyreports/exception.py` & `pyreports-1.7.0/pyreports/exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # exception.py -- pyreports
 #
-#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2024 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -24,15 +24,19 @@
 
 
 class ExecutorError(Exception):
     pass
 
 
 # ReportException hierarchy
-class ReportException(Exception):
+class DataObjectError(Exception):
+    pass
+
+
+class ReportException(DataObjectError):
     pass
 
 
 class ReportDataError(ReportException):
     pass
```

### Comparing `pyreports-1.6.0/pyreports/io.py` & `pyreports-1.7.0/pyreports/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 # vim: se ts=4 et syn=python:
 
 # created by: matteo.guadrini
 # io -- pyreports
 #
-#     Copyright (C) 2023 Matteo Guadrini <matteo.guadrini@hotmail.it>
+#     Copyright (C) 2024 Matteo Guadrini <matteo.guadrini@hotmail.it>
 #
 #     This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
@@ -22,15 +22,14 @@
 
 """Contains all input management."""
 
 # region Imports
 import sqlite3
 from typing import Union, List
 import nosqlapi
-import pymssql
 import mysql.connector as mdb
 import psycopg2
 import tablib
 import ldap3
 import re
 from nosqlapi import Manager as APIManager
 from nosqlapi import Connection as APIConnection
@@ -110,58 +109,59 @@
         with open(self.file) as file:
             for line in file:
                 yield line
 
 
 class Manager(ABC):
     """Manager base class"""
+
     pass
 
 
 class TextFile(File):
     """Text file class"""
 
     def write(self, data):
         """Write data on file
 
         :param data: data to write on file
         :return: None
         """
         if not isinstance(data, tablib.Dataset):
             data = tablib.Dataset(data)
-        with open(self.file, mode='w') as file:
-            file.write('\n'.join(str(line) for row in data for line in row))
+        with open(self.file, mode="w") as file:
+            file.write("\n".join(str(line) for row in data for line in row))
 
     def read(self, **kwargs):
         """Read with format
 
         :return: Dataset object
         """
         data = tablib.Dataset(**kwargs)
         with open(self.file) as file:
             for line in file:
-                data.append([line.strip('\n')])
+                data.append([line.strip("\n")])
         return data
 
 
 class LogFile(File):
     """Log file class"""
 
     def write(self, data):
         """Write data on file
 
         :param data: data to write on file
         :return: None
         """
         if not isinstance(data, tablib.Dataset):
             data = tablib.Dataset(*data)
-        with open(self.file, mode='w') as file:
-            file.write('\n'.join([' '.join(row).strip('\n') for row in data]))
+        with open(self.file, mode="w") as file:
+            file.write("\n".join([" ".join(row).strip("\n") for row in data]))
 
-    def read(self, pattern=r'(.*\n|.*$)', **kwargs):
+    def read(self, pattern=r"(.*\n|.*$)", **kwargs):
         """Read with format
 
         :param pattern: regular expression pattern
         :return: Dataset object
         """
         data = tablib.Dataset(**kwargs)
         with open(self.file) as file:
@@ -182,16 +182,16 @@
         """Write data on csv file
 
         :param data: data to write on csv file
         :return: None
         """
         if not isinstance(data, tablib.Dataset):
             data = tablib.Dataset(data)
-        with open(self.file, mode='w') as file:
-            file.write(data.export('csv'))
+        with open(self.file, mode="w") as file:
+            file.write(data.export("csv"))
 
     def read(self, **kwargs):
         """Read csv format
 
         :return: Dataset object
         """
         with open(self.file) as file:
@@ -205,16 +205,16 @@
         """Write data on json file
 
         :param data: data to write on json file
         :return: None
         """
         if not isinstance(data, tablib.Dataset):
             data = tablib.Dataset(data)
-        with open(self.file, mode='w') as file:
-            file.write(data.export('json'))
+        with open(self.file, mode="w") as file:
+            file.write(data.export("json"))
 
     def read(self, **kwargs):
         """Read json format
 
         :return: Dataset object
         """
         with open(self.file) as file:
@@ -228,16 +228,16 @@
         """Write data on yaml file
 
         :param data: data to write on yaml file
         :return: None
         """
         if not isinstance(data, tablib.Dataset):
             data = tablib.Dataset(data)
-        with open(self.file, mode='w') as file:
-            file.write(data.export('yaml'))
+        with open(self.file, mode="w") as file:
+            file.write(data.export("yaml"))
 
     def read(self, **kwargs):
         """Read yaml format
 
         :return: Dataset object
         """
         with open(self.file) as file:
@@ -251,23 +251,23 @@
         """Write data on xlsx file
 
         :param data: data to write on yaml file
         :return: None
         """
         if not isinstance(data, tablib.Dataset):
             data = tablib.Dataset(data)
-        with open(self.file, mode='wb') as file:
-            file.write(data.export('xlsx'))
+        with open(self.file, mode="wb") as file:
+            file.write(data.export("xlsx"))
 
     def read(self, **kwargs):
         """Read xlsx format
 
         :return: Dataset object
         """
-        with open(self.file, 'rb') as file:
+        with open(self.file, "rb") as file:
             return tablib.import_set(file, **kwargs)
 
 
 class SQLiteConnection(Connection):
     """Connection sqlite class"""
 
     def connect(self):
@@ -275,26 +275,14 @@
         self.cursor = self.connection.cursor()
 
     def close(self):
         self.connection.close()
         self.cursor.close()
 
 
-class MSSQLConnection(Connection):
-    """Connection microsoft sql class"""
-
-    def connect(self):
-        self.connection = pymssql.connect(*self.args, **self.kwargs)
-        self.cursor = self.connection.cursor()
-
-    def close(self):
-        self.connection.close()
-        self.cursor.close()
-
-
 class MySQLConnection(Connection):
     """Connection mysql class"""
 
     def connect(self):
         self.connection = mdb.connect(*self.args, **self.kwargs)
         self.cursor = self.connection.cursor()
 
@@ -319,15 +307,15 @@
     """Database manager class for SQL connection"""
 
     def __init__(self, connection: Connection):
         """Database manager object for SQL connection
 
         :param connection: Connection based object
         """
-        self.type = 'sql'
+        self.type = "sql"
         self.connector = connection
         # Connect database
         self.connector.connect()
         # Set description
         self.description = None
         self.data = None
         # Row properties
@@ -406,15 +394,17 @@
 
     def fetchone(self) -> tablib.Dataset:
         """Retrieves the next row of a query result set
 
         :return: Dataset object
         """
         header = [field[0] for field in self.description]
-        self.data = tablib.Dataset(list(self.connector.cursor.fetchone()), headers=header)
+        self.data = tablib.Dataset(
+            list(self.connector.cursor.fetchone()), headers=header
+        )
         return self.data
 
     def fetchmany(self, size=1) -> tablib.Dataset:
         """Fetches the next set of rows of a query result
 
         :param size: the number of rows returned
         :return: Dataset object
@@ -449,31 +439,33 @@
 
 
 class NoSQLManager(Manager, APIManager):
     """Database manager class for NOSQL connection"""
 
     def __init__(self, connection: APIConnection, *args, **kwargs):
         APIManager.__init__(self, connection, *args, **kwargs)
-        self.type = 'nosql'
+        self.type = "nosql"
 
     @staticmethod
     def _response_to_dataset(
-            obj: Union[List[tuple], List[list], dict, nosqlapi.Response]
+        obj: Union[List[tuple], List[list], dict, nosqlapi.Response],
     ) -> tablib.Dataset:
         """Transform receive data into Dataset object"""
         data = tablib.Dataset()
         if isinstance(obj, (list, tuple)):
             data = tablib.Dataset([row for row in obj])
         elif isinstance(obj, dict):
             data = tablib.Dataset([obj[key] for key in obj], headers=list(obj.keys()))
         elif isinstance(obj, nosqlapi.Response):
             if isinstance(obj.data, (list, tuple)):
                 data = tablib.Dataset([row for row in obj.data])
             elif isinstance(obj.data, dict):
-                data = tablib.Dataset([obj.data[key] for key in obj], headers=list(obj.data.keys()))
+                data = tablib.Dataset(
+                    [obj.data[key] for key in obj], headers=list(obj.data.keys())
+                )
         else:
             data.append(obj)
 
         return data
 
     def get(self, *args, **kwargs) -> tablib.Dataset:
         """Get data from database session"""
@@ -488,15 +480,15 @@
     """File manager class for various readable file format"""
 
     def __init__(self, file: File):
         """File manager object for various readable file format
 
         :param file: file object
         """
-        self.type = 'file'
+        self.type = "file"
         self.data = file
 
     def __repr__(self):
         """Representation of FileManager object
 
         :return: string
         """
@@ -535,26 +527,32 @@
 
         :param server: fqdn server name or ip address
         :param username: username for bind operation
         :param password: password of the username used for bind operation
         :param ssl: disable or enable SSL. Default is False.
         :param tls: disable or enable TLS. Default is True.
         """
-        self.type = 'ldap'
+        self.type = "ldap"
         # Check ssl connection
         port = 636 if ssl else 389
-        self.connector = ldap3.Server(server,
-                                      get_info=ldap3.ALL,
-                                      port=port,
-                                      use_ssl=ssl)
+        self.connector = ldap3.Server(
+            server, get_info=ldap3.ALL, port=port, use_ssl=ssl
+        )
         # Check tls connection
-        self.auto_bind = ldap3.AUTO_BIND_TLS_BEFORE_BIND if tls else ldap3.AUTO_BIND_NONE
+        self.auto_bind = (
+            ldap3.AUTO_BIND_TLS_BEFORE_BIND if tls else ldap3.AUTO_BIND_NONE
+        )
         # Create a bind connection with user and password
-        self.bind = ldap3.Connection(self.connector, user=f'{username}', password=f'{password}',
-                                     auto_bind=self.auto_bind, raise_exceptions=True)
+        self.bind = ldap3.Connection(
+            self.connector,
+            user=f"{username}",
+            password=f"{password}",
+            auto_bind=self.auto_bind,
+            raise_exceptions=True,
+        )
         self.bind.bind()
 
     def __repr__(self):
         """Representation of LdapManager object
 
         :return: string
         """
@@ -568,16 +566,21 @@
 
         :param username: username for bind operation
         :param password: password of the username used for bind operation
         :return: None
         """
         # Disconnect LDAP server
         self.bind.unbind()
-        self.bind = ldap3.Connection(self.connector, user=f'{username}', password=f'{password}',
-                                     auto_bind=self.auto_bind, raise_exceptions=True)
+        self.bind = ldap3.Connection(
+            self.connector,
+            user=f"{username}",
+            password=f"{password}",
+            auto_bind=self.auto_bind,
+            raise_exceptions=True,
+        )
         self.bind.bind()
 
     def unbind(self):
         """Unbind LDAP connection
 
         :return: None
         """
@@ -587,52 +590,55 @@
         """Search LDAP element on subtree base search directory
 
         :param base_search: distinguishedName of LDAP base search
         :param search_filter: LDAP query language
         :param attributes: list of returning LDAP attributes
         :return: Dataset object
         """
-        if self.bind.search(search_base=base_search, search_filter=f'{search_filter}', attributes=attributes,
-                            search_scope=ldap3.SUBTREE):
+        if self.bind.search(
+            search_base=base_search,
+            search_filter=f"{search_filter}",
+            attributes=attributes,
+            search_scope=ldap3.SUBTREE,
+        ):
             # Build Dataset
             data = tablib.Dataset()
             data.headers = attributes
             for result in self.bind.response:
-                if result.get('attributes'):
+                if result.get("attributes"):
                     row = list()
                     for index, _ in enumerate(attributes):
-                        row.append(result.get('attributes').get(attributes[index]))
+                        row.append(result.get("attributes").get(attributes[index]))
                     data.append(row)
             # Return object
             return data
 
 
 # endregion
 
 
 # region Variables
 DBTYPE = {
-    'sqlite': SQLiteConnection,
-    'mssql': MSSQLConnection,
-    'mysql': MySQLConnection,
-    'postgresql': PostgreSQLConnection
+    "sqlite": SQLiteConnection,
+    "mysql": MySQLConnection,
+    "postgresql": PostgreSQLConnection,
 }
 
 FILETYPE = {
-    'file': TextFile,
-    'log': LogFile,
-    'csv': CsvFile,
-    'json': JsonFile,
-    'yaml': YamlFile,
-    'xlsx': ExcelFile,
+    "file": TextFile,
+    "log": LogFile,
+    "csv": CsvFile,
+    "json": JsonFile,
+    "yaml": YamlFile,
+    "xlsx": ExcelFile,
 }
 
-READABLE_MANAGER = ('FileManager', 'DatabaseManager', 'LdapManager', 'NoSQLManager')
+READABLE_MANAGER = ("FileManager", "DatabaseManager", "LdapManager", "NoSQLManager")
 
-WRITABLE_MANAGER = ('FileManager', 'DatabaseManager', 'NoSQLManager')
+WRITABLE_MANAGER = ("FileManager", "DatabaseManager", "NoSQLManager")
 
 
 # endregion
 
 
 # region Functions
 def create_database_manager(dbtype, *args, **kwargs):
@@ -674,16 +680,18 @@
 def create_nosql_manager(connection, *args, **kwargs):
     """Creates a NoSQLManager object
 
     :param connection: Connection object
     :return: NoSQLManager
     """
     # Check if connection class is API compliant with nosqlapi
-    if not hasattr(connection, 'connect'):
-        raise nosqlapi.ConnectError('the Connection class is not API compliant. See https://nosqlapi.rtfd.io/')
+    if not hasattr(connection, "connect"):
+        raise nosqlapi.ConnectError(
+            "the Connection class is not API compliant. See https://nosqlapi.rtfd.io/"
+        )
     # Create NoSQLManager object
     return NoSQLManager(connection=connection, *args, **kwargs)
 
 
 def manager(datatype, *args, **kwargs):
     """Creates manager object based on datatype
 
@@ -693,21 +701,22 @@
     :return: Manager object
     """
     # Choose manager type
     if datatype in DBTYPE:
         return create_database_manager(datatype, *args, **kwargs)
     elif datatype in FILETYPE:
         return create_file_manager(datatype, *args, **kwargs)
-    elif datatype == 'ldap':
+    elif datatype == "ldap":
         return create_ldap_manager(*args, **kwargs)
-    elif datatype == 'nosql':
-        connection = kwargs.get('connection') or args[0]
+    elif datatype == "nosql":
+        connection = kwargs.get("connection") or args[0]
         nargs = args[1:]
         try:
-            kwargs.pop('connection')
+            kwargs.pop("connection")
         except KeyError:
             pass
         return create_nosql_manager(connection, *nargs, **kwargs)
     else:
         raise ValueError(f"data type {datatype} doesn't exists!")
 
+
 # endregion
```

### Comparing `pyreports-1.6.0/pyreports.egg-info/PKG-INFO` & `pyreports-1.7.0/pyreports.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 Metadata-Version: 2.1
 Name: pyreports
-Version: 1.6.0
+Version: 1.7.0
 Summary: pyreports is a python library that allows you to create complex report from various sources.
 Home-page: https://github.com/MatteoGuadrini/pyreports
 Author: Matteo Guadrini
 Author-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 Maintainer: Matteo Guadrini
 Maintainer-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 License: GNU General Public License v3.0
 Project-URL: homepage, https://github.com/MatteoGuadrini/pyreports'
 Project-URL: documentation, https://pyreports.readthedocs.io/en/latest/
-Project-URL: repository, https://github.com/MatteoGuadrini/pyreports/pyreports.git
+Project-URL: repository, https://github.com/MatteoGuadrini/pyreports.git
 Project-URL: changelog, https://github.com/MatteoGuadrini/pyreports/blob/master/CHANGES.md
 Keywords: pyreports,reports,report,csv,yaml,export,excel,database,ldap,dataset,file,executor,book
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: ldap3
+Requires-Dist: mysql-connector-python
+Requires-Dist: psycopg2-binary
+Requires-Dist: tablib
+Requires-Dist: tablib[all]
+Requires-Dist: nosqlapi
+Requires-Dist: pyyaml
 
 # pyreports
 
 <img src="https://pyreports.readthedocs.io/en/latest/_static/pyreports.svg" alt="pyreports" title="pyreports" width="300" height="300" />
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/2bad30d308414c83836f22f012c98649)](https://www.codacy.com/gh/MatteoGuadrini/pyreports/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=MatteoGuadrini/pyreports&amp;utm_campaign=Badge_Grade)
 [![CircleCI](https://circleci.com/gh/MatteoGuadrini/pyreports.svg?style=svg)](https://circleci.com/gh/MatteoGuadrini/pyreports)
```

### Comparing `pyreports-1.6.0/pyreports.egg-info/SOURCES.txt` & `pyreports-1.7.0/pyreports.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.readthedocs.yaml
 CHANGES.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE.md
 MANIFEST.in
 README.md
 favicon.ico
```

### Comparing `pyreports-1.6.0/setup.py` & `pyreports-1.7.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from setuptools import setup
 
 
-__version__ = '1.6.0'
-__author__ = 'Matteo Guadrini'
-__email__ = 'matteo.guadrini@hotmail.it'
-__homepage__ = 'https://github.com/MatteoGuadrini/pyreports'
+__version__ = "1.6.0"
+__author__ = "Matteo Guadrini"
+__email__ = "matteo.guadrini@hotmail.it"
+__homepage__ = "https://github.com/MatteoGuadrini/pyreports"
 
 with open("README.md") as rme, open("CHANGES.md") as ch:
     long_description = rme.read() + "\n" + ch.read()
 
 setup(
-    name='pyreports',
+    name="pyreports",
     version=__version__,
-    packages=['pyreports'],
+    packages=["pyreports"],
     url=__homepage__,
-    license='GNU General Public License v3.0',
+    license="GNU General Public License v3.0",
     author=__author__,
     author_email=__email__,
-    keywords='pyreports reports report csv yaml export excel database ldap dataset file executor book',
-    maintainer='Matteo Guadrini',
-    maintainer_email='matteo.guadrini@hotmail.it',
-    install_requires=['ldap3', 'pymssql', 'mysql-connector-python',
-                      'psycopg2-binary', 'tablib', 'tablib[all]', 'nosqlapi', 'pyyaml'],
-    description='pyreports is a python library that allows you to create complex report from various sources',
+    keywords="pyreports reports report csv yaml export excel database ldap dataset file executor book",
+    maintainer="Matteo Guadrini",
+    maintainer_email="matteo.guadrini@hotmail.it",
+    install_requires=[
+        "ldap3",
+        "mysql-connector-python",
+        "psycopg2-binary",
+        "tablib",
+        "tablib[all]",
+        "nosqlapi",
+        "pyyaml",
+    ],
+    description="pyreports is a python library that allows you to create complex report from various sources",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
-            "Programming Language :: Python :: 3",
-            "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-            "Operating System :: OS Independent",
-        ],
-    entry_points={
-        'console_scripts': [
-            'reports = pyreports.cli:main'
-        ]
-    },
-    python_requires='>=3.7'
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Operating System :: OS Independent",
+    ],
+    entry_points={"console_scripts": ["reports = pyreports.cli:main"]},
+    python_requires=">=3.7",
 )
```

### Comparing `pyreports-1.6.0/tests/__init__.py` & `pyreports-1.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/tests/test_core.py` & `pyreports-1.7.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyreports-1.6.0/tests/test_db.py` & `pyreports-1.7.0/tests/test_db.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,155 +1,133 @@
 import unittest
 import pyreports
 from tablib import Dataset
 from unittest.mock import MagicMock, patch
 
 
 class TestDBConnection(unittest.TestCase):
-
     def test_connection(self):
         # pyreports.io.Connection object
         self.assertRaises(TypeError, pyreports.io.Connection)
 
     def test_sqllite_connection(self):
         # Simulate pyreports.io.SQLliteConnection object
         conn = MagicMock()
-        with patch(target='sqlite3.connect') as mock:
+        with patch(target="sqlite3.connect") as mock:
             # Test connect
             conn.connection = mock.return_value
             conn.cursor = conn.connection.cursor.return_value
-            conn.connection.database = 'mydb.db'
-            self.assertEqual(conn.connection.database, 'mydb.db')
+            conn.connection.database = "mydb.db"
+            self.assertEqual(conn.connection.database, "mydb.db")
             # Test close
             conn.cursor.close()
 
     def test_mysql_connection(self):
         # Simulate pyreports.io.MySQLConnection object
         conn = MagicMock()
-        with patch(target='mysql.connector.connect') as mock:
+        with patch(target="mysql.connector.connect") as mock:
             # Test connect
             conn.connection = mock.return_value
             conn.cursor = conn.connection.cursor.return_value
-            conn.connection.host = 'mysqldb.local'
-            conn.connection.database = 'mydb'
-            conn.connection.username = 'username'
-            conn.connection.password = 'password'
+            conn.connection.host = "mysqldb.local"
+            conn.connection.database = "mydb"
+            conn.connection.username = "username"
+            conn.connection.password = "password"
             conn.connection.port = 3306
-            self.assertEqual(conn.connection.host, 'mysqldb.local')
-            self.assertEqual(conn.connection.database, 'mydb')
-            self.assertEqual(conn.connection.username, 'username')
-            self.assertEqual(conn.connection.password, 'password')
+            self.assertEqual(conn.connection.host, "mysqldb.local")
+            self.assertEqual(conn.connection.database, "mydb")
+            self.assertEqual(conn.connection.username, "username")
+            self.assertEqual(conn.connection.password, "password")
             self.assertEqual(conn.connection.port, 3306)
             # Test close
             conn.cursor.close()
 
-    def test_mssqldb_connection(self):
-        # Simulate pyreports.io.MSSQLConnection object
-        conn = MagicMock()
-        with patch(target='pymssql.connect') as mock:
-            # Test connect
-            conn.connection = mock.return_value
-            conn.cursor = conn.connection.cursor.return_value
-            conn.connection.host = 'mssqldb.local'
-            conn.connection.database = 'mydb'
-            conn.connection.username = 'username'
-            conn.connection.password = 'password'
-            conn.connection.port = 1433
-            self.assertEqual(conn.connection.host, 'mssqldb.local')
-            self.assertEqual(conn.connection.database, 'mydb')
-            self.assertEqual(conn.connection.username, 'username')
-            self.assertEqual(conn.connection.password, 'password')
-            self.assertEqual(conn.connection.port, 1433)
-            # Test close
-            conn.cursor.close()
-
     def test_postgresqldb_connection(self):
         # Simulate pyreports.io.PostgreSQLConnection object
         conn = MagicMock()
-        with patch(target='psycopg2.connect') as mock:
+        with patch(target="psycopg2.connect") as mock:
             # Test connect
             conn.connection = mock.return_value
             conn.cursor = conn.connection.cursor.return_value
-            conn.connection.host = 'postgresqldb.local'
-            conn.connection.database = 'mydb'
-            conn.connection.username = 'username'
-            conn.connection.password = 'password'
+            conn.connection.host = "postgresqldb.local"
+            conn.connection.database = "mydb"
+            conn.connection.username = "username"
+            conn.connection.password = "password"
             conn.connection.port = 5432
-            self.assertEqual(conn.connection.host, 'postgresqldb.local')
-            self.assertEqual(conn.connection.database, 'mydb')
-            self.assertEqual(conn.connection.username, 'username')
-            self.assertEqual(conn.connection.password, 'password')
+            self.assertEqual(conn.connection.host, "postgresqldb.local")
+            self.assertEqual(conn.connection.database, "mydb")
+            self.assertEqual(conn.connection.username, "username")
+            self.assertEqual(conn.connection.password, "password")
             self.assertEqual(conn.connection.port, 5432)
             # Test close
             conn.cursor.close()
 
 
 class TestDBManager(unittest.TestCase):
-
     conn = MagicMock()
-    with patch(target='psycopg2.connect') as mock:
+    with patch(target="psycopg2.connect") as mock:
         conn.connection = mock.return_value
         conn.cursor = conn.connection.cursor.return_value
-        conn.connection.host = 'postgresqldb.local'
-        conn.connection.database = 'mydb'
-        conn.connection.username = 'username'
-        conn.connection.password = 'password'
+        conn.connection.host = "postgresqldb.local"
+        conn.connection.database = "mydb"
+        conn.connection.username = "username"
+        conn.connection.password = "password"
         conn.connection.port = 5432
 
     def test_db_manager(self):
         # Test database manager
         db_manager = pyreports.io.DatabaseManager(connection=self.conn)
         self.assertIsInstance(db_manager, pyreports.io.DatabaseManager)
         # Test reconnect
         db_manager.reconnect()
         # Test SELECT query
-        db_manager.execute('SELECT * from test')
+        db_manager.execute("SELECT * from test")
         data = db_manager.fetchall()
         self.assertIsInstance(data, Dataset)
         # Test store procedure
-        db_manager.callproc('myproc')
+        db_manager.callproc("myproc")
         data = db_manager.fetchone()
         self.assertIsInstance(data, Dataset)
 
 
 class TestNoSQLManager(unittest.TestCase):
-
     conn = MagicMock()
-    with patch(target='nosqlapi.Connection') as mock:
+    with patch(target="nosqlapi.Connection") as mock:
         conn.connection = mock.return_value
         conn.session = conn.connection.connect()
-        conn.connection.host = 'mongodb.local'
-        conn.connection.database = 'mydb'
-        conn.connection.username = 'username'
-        conn.connection.password = 'password'
+        conn.connection.host = "mongodb.local"
+        conn.connection.database = "mydb"
+        conn.connection.username = "username"
+        conn.connection.password = "password"
         conn.connection.port = 27017
 
     def test_nosql_manager(self):
         # Test nosql database manager
         nosql_manager = pyreports.io.NoSQLManager(connection=self.conn)
         self.assertIsInstance(nosql_manager, pyreports.io.NoSQLManager)
         # Test get data
-        data = nosql_manager.get('doc1')
+        data = nosql_manager.get("doc1")
         self.assertIsInstance(data, Dataset)
         # Test find data
         data = nosql_manager.find({"name": "Arthur"})
         self.assertIsInstance(data, Dataset)
 
 
 class TestLDAPManager(unittest.TestCase):
-
     conn = MagicMock()
-    with patch(target='ldap3.Server') as mock:
+    with patch(target="ldap3.Server") as mock:
         conn.connector = mock.return_value
-    with patch(target='ldap3.Connection') as mock:
+    with patch(target="ldap3.Connection") as mock:
         conn.bind = mock.return_value
 
     def test_bind(self):
         self.conn.bind.bind()
         self.conn.bind.unbind()
 
     def test_query(self):
-        self.conn.bind.search('OU=test,DC=test,DC=local', 'objectCategory=person', ['name', 'sn', 'phone'])
+        self.conn.bind.search(
+            "OU=test,DC=test,DC=local", "objectCategory=person", ["name", "sn", "phone"]
+        )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `pyreports-1.6.0/tests/test_file.py` & `pyreports-1.7.0/tests/test_file.py`

 * *Files identical despite different names*

