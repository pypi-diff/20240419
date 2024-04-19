# Comparing `tmp/pyDetektia-1.0.1.tar.gz` & `tmp/pyDetektia-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDetektia-1.0.1.tar", last modified: Thu Nov  9 15:59:04 2023, max compression
+gzip compressed data, was "pyDetektia-2.0.0.tar", last modified: Fri Apr 19 13:26:08 2024, max compression
```

## Comparing `pyDetektia-1.0.1.tar` & `pyDetektia-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2023-11-09 15:59:04.110297 pyDetektia-1.0.1/
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        0 2023-06-19 12:15:27.000000 pyDetektia-1.0.1/LICENSE.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      326 2023-11-09 15:59:04.110297 pyDetektia-1.0.1/PKG-INFO
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       13 2023-09-05 11:56:56.000000 pyDetektia-1.0.1/README.md
-drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2023-11-09 15:59:04.110297 pyDetektia-1.0.1/pyDetektia/
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        0 2022-07-11 08:00:56.000000 pyDetektia-1.0.1/pyDetektia/__init__.py
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)    27842 2023-11-09 15:35:26.000000 pyDetektia-1.0.1/pyDetektia/manager.py
-drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2023-11-09 15:59:04.110297 pyDetektia-1.0.1/pyDetektia.egg-info/
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      326 2023-11-09 15:59:04.000000 pyDetektia-1.0.1/pyDetektia.egg-info/PKG-INFO
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      244 2023-11-09 15:59:04.000000 pyDetektia-1.0.1/pyDetektia.egg-info/SOURCES.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        1 2023-11-09 15:59:04.000000 pyDetektia-1.0.1/pyDetektia.egg-info/dependency_links.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        9 2023-11-09 15:59:04.000000 pyDetektia-1.0.1/pyDetektia.egg-info/requires.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       11 2023-11-09 15:59:04.000000 pyDetektia-1.0.1/pyDetektia.egg-info/top_level.txt
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       38 2023-11-09 15:59:04.110297 pyDetektia-1.0.1/setup.cfg
--rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      464 2023-11-09 15:43:08.000000 pyDetektia-1.0.1/setup.py
+drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-04-19 13:26:08.478669 pyDetektia-2.0.0/
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        0 2023-06-19 12:15:27.000000 pyDetektia-2.0.0/LICENSE.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      326 2024-04-19 13:26:08.478669 pyDetektia-2.0.0/PKG-INFO
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       13 2023-09-05 11:56:56.000000 pyDetektia-2.0.0/README.md
+drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-04-19 13:26:08.478669 pyDetektia-2.0.0/pyDetektia/
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        0 2022-07-11 08:00:56.000000 pyDetektia-2.0.0/pyDetektia/__init__.py
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)    45611 2024-04-19 13:07:38.000000 pyDetektia-2.0.0/pyDetektia/manager.py
+drwxrwxr-x   0 alvaro    (1000) alvaro    (1001)        0 2024-04-19 13:26:08.478669 pyDetektia-2.0.0/pyDetektia.egg-info/
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      326 2024-04-19 13:26:08.000000 pyDetektia-2.0.0/pyDetektia.egg-info/PKG-INFO
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      244 2024-04-19 13:26:08.000000 pyDetektia-2.0.0/pyDetektia.egg-info/SOURCES.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        1 2024-04-19 13:26:08.000000 pyDetektia-2.0.0/pyDetektia.egg-info/dependency_links.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)        9 2024-04-19 13:26:08.000000 pyDetektia-2.0.0/pyDetektia.egg-info/requires.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       11 2024-04-19 13:26:08.000000 pyDetektia-2.0.0/pyDetektia.egg-info/top_level.txt
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)       38 2024-04-19 13:26:08.478669 pyDetektia-2.0.0/setup.cfg
+-rw-rw-r--   0 alvaro    (1000) alvaro    (1001)      464 2024-04-19 13:08:00.000000 pyDetektia-2.0.0/setup.py
```

