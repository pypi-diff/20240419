# Comparing `tmp/sfmanager-0.0.9.tar.gz` & `tmp/sfmanager-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfmanager-0.0.9.tar", last modified: Thu Apr 18 15:02:02 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sfmanager-0.0.9.tar` & `sfmanager-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,7 @@
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 15:02:02.656167 sfmanager-0.0.9/
--rw-rw-r--   0 grand     (1000) grand     (1000)      887 2024-04-18 15:02:02.656167 sfmanager-0.0.9/PKG-INFO
--rw-rw-r--   0 grand     (1000) grand     (1000)      365 2024-04-18 05:45:03.000000 sfmanager-0.0.9/README.md
--rw-rw-r--   0 grand     (1000) grand     (1000)       38 2024-04-18 15:02:02.660167 sfmanager-0.0.9/setup.cfg
--rw-rw-r--   0 grand     (1000) grand     (1000)      822 2024-04-18 10:08:46.000000 sfmanager-0.0.9/setup.py
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 15:02:02.652167 sfmanager-0.0.9/sfmanager/
--rw-rw-r--   0 grand     (1000) grand     (1000)       73 2024-04-18 06:32:48.000000 sfmanager-0.0.9/sfmanager/__init__.py
--rw-rw-r--   0 grand     (1000) grand     (1000)     3392 2024-04-18 14:37:28.000000 sfmanager-0.0.9/sfmanager/app.py
--rw-rw-r--   0 grand     (1000) grand     (1000)       75 2024-04-18 14:38:11.000000 sfmanager-0.0.9/sfmanager/test.py
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 15:02:02.656167 sfmanager-0.0.9/sfmanager.egg-info/
--rw-rw-r--   0 grand     (1000) grand     (1000)      887 2024-04-18 15:02:02.000000 sfmanager-0.0.9/sfmanager.egg-info/PKG-INFO
--rw-rw-r--   0 grand     (1000) grand     (1000)      249 2024-04-18 15:02:02.000000 sfmanager-0.0.9/sfmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)        1 2024-04-18 15:02:02.000000 sfmanager-0.0.9/sfmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)       31 2024-04-18 15:02:02.000000 sfmanager-0.0.9/sfmanager.egg-info/requires.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)       10 2024-04-18 15:02:02.000000 sfmanager-0.0.9/sfmanager.egg-info/top_level.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 sfmanager-0.1.0/sfmanager/__init__.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 sfmanager-0.1.0/sfmanager/app.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 sfmanager-0.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sfmanager-0.1.0/LICENSE
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 sfmanager-0.1.0/README.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 sfmanager-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 sfmanager-0.1.0/PKG-INFO
```

### Comparing `sfmanager-0.0.9/sfmanager/app.py` & `sfmanager-0.1.0/sfmanager/app.py`

 * *Files identical despite different names*

