# Comparing `tmp/exenake-0.0.1.tar.gz` & `tmp/exenake-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exenake-0.0.1.tar", last modified: Fri Apr 19 12:28:39 2024, max compression
+gzip compressed data, was "exenake-0.0.2.tar", last modified: Fri Apr 19 12:44:54 2024, max compression
```

## Comparing `exenake-0.0.1.tar` & `exenake-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 12:28:39.613673 exenake-0.0.1/
--rw-rw-rw-   0        0        0      322 2024-04-19 12:28:39.613673 exenake-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-19 12:28:39.612673 exenake-0.0.1/exeNake.egg-info/
--rw-rw-rw-   0        0        0      322 2024-04-19 12:28:39.000000 exenake-0.0.1/exeNake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      132 2024-04-19 12:28:39.000000 exenake-0.0.1/exeNake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 12:28:39.000000 exenake-0.0.1/exeNake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 12:28:39.000000 exenake-0.0.1/exeNake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 12:28:39.613673 exenake-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      448 2024-04-19 12:28:38.000000 exenake-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 12:44:54.084965 exenake-0.0.2/
+-rw-rw-rw-   0        0        0      322 2024-04-19 12:44:54.083964 exenake-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 12:44:54.083964 exenake-0.0.2/exeNake.egg-info/
+-rw-rw-rw-   0        0        0      322 2024-04-19 12:44:54.000000 exenake-0.0.2/exeNake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      132 2024-04-19 12:44:54.000000 exenake-0.0.2/exeNake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 12:44:54.000000 exenake-0.0.2/exeNake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 12:44:54.000000 exenake-0.0.2/exeNake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 12:44:54.084965 exenake-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      448 2024-04-19 12:44:30.000000 exenake-0.0.2/setup.py
```

