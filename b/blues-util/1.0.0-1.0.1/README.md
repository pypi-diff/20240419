# Comparing `tmp/blues_util-1.0.0.tar.gz` & `tmp/blues_util-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blues_util-1.0.0.tar", last modified: Fri Apr 19 17:07:03 2024, max compression
+gzip compressed data, was "blues_util-1.0.1.tar", last modified: Fri Apr 19 17:37:44 2024, max compression
```

## Comparing `blues_util-1.0.0.tar` & `blues_util-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 17:07:03.150097 blues_util-1.0.0/
--rw-rw-rw-   0        0        0       77 2024-04-19 17:07:03.148696 blues_util-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 17:07:03.148696 blues_util-1.0.0/blues_util.egg-info/
--rw-rw-rw-   0        0        0       77 2024-04-19 17:07:03.000000 blues_util-1.0.0/blues_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      144 2024-04-19 17:07:03.000000 blues_util-1.0.0/blues_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 17:07:03.000000 blues_util-1.0.0/blues_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 17:07:03.000000 blues_util-1.0.0/blues_util.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 17:07:03.150097 blues_util-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      260 2024-04-19 16:39:22.000000 blues_util-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:37:44.867850 blues_util-1.0.1/
+-rw-rw-rw-   0        0        0       77 2024-04-19 17:37:44.867850 blues_util-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       35 2024-04-19 17:33:13.000000 blues_util-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 17:37:44.867850 blues_util-1.0.1/blues_util.egg-info/
+-rw-rw-rw-   0        0        0       77 2024-04-19 17:37:44.000000 blues_util-1.0.1/blues_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-04-19 17:37:44.000000 blues_util-1.0.1/blues_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 17:37:44.000000 blues_util-1.0.1/blues_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 17:37:44.000000 blues_util-1.0.1/blues_util.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-19 17:37:44.867850 blues_util-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      260 2024-04-19 17:35:49.000000 blues_util-1.0.1/setup.py
```

