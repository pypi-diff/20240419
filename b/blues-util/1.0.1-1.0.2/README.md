# Comparing `tmp/blues_util-1.0.1.tar.gz` & `tmp/blues_util-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blues_util-1.0.1.tar", last modified: Fri Apr 19 17:37:44 2024, max compression
+gzip compressed data, was "blues_util-1.0.2.tar", last modified: Fri Apr 19 17:41:52 2024, max compression
```

## Comparing `blues_util-1.0.1.tar` & `blues_util-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 17:37:44.867850 blues_util-1.0.1/
--rw-rw-rw-   0        0        0       77 2024-04-19 17:37:44.867850 blues_util-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       35 2024-04-19 17:33:13.000000 blues_util-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 17:37:44.867850 blues_util-1.0.1/blues_util.egg-info/
--rw-rw-rw-   0        0        0       77 2024-04-19 17:37:44.000000 blues_util-1.0.1/blues_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      164 2024-04-19 17:37:44.000000 blues_util-1.0.1/blues_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 17:37:44.000000 blues_util-1.0.1/blues_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 17:37:44.000000 blues_util-1.0.1/blues_util.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-19 17:37:44.867850 blues_util-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      260 2024-04-19 17:35:49.000000 blues_util-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 17:41:52.752407 blues_util-1.0.2/
+-rw-rw-rw-   0        0        0       77 2024-04-19 17:41:52.752407 blues_util-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       35 2024-04-19 17:33:13.000000 blues_util-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-19 17:41:52.752019 blues_util-1.0.2/blues_util.egg-info/
+-rw-rw-rw-   0        0        0       77 2024-04-19 17:41:52.000000 blues_util-1.0.2/blues_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-04-19 17:41:52.000000 blues_util-1.0.2/blues_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 17:41:52.000000 blues_util-1.0.2/blues_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 17:41:52.000000 blues_util-1.0.2/blues_util.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-19 17:41:52.755114 blues_util-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      260 2024-04-19 17:41:13.000000 blues_util-1.0.2/setup.py
```

