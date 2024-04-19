# Comparing `tmp/pih-bonus-0.1.tar.gz` & `tmp/pih-bonus-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-bonus-0.1.tar", last modified: Wed Apr 10 01:35:46 2024, max compression
+gzip compressed data, was "pih-bonus-0.11.tar", last modified: Fri Apr 19 02:21:12 2024, max compression
```

## Comparing `pih-bonus-0.1.tar` & `pih-bonus-0.11.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 01:35:46.346552 pih-bonus-0.1/
-drwxrwxrwx   0        0        0        0 2024-04-10 01:35:45.939267 pih-bonus-0.1/BonusProgramService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-bonus-0.1/BonusProgramService/__init__.py
--rw-rw-rw-   0        0        0      154 2024-04-09 22:47:56.000000 pih-bonus-0.1/BonusProgramService/__main__.py
--rw-rw-rw-   0        0        0      399 2024-04-09 22:46:01.000000 pih-bonus-0.1/BonusProgramService/const.py
--rw-rw-rw-   0        0        0     1752 2024-04-09 22:46:59.000000 pih-bonus-0.1/BonusProgramService/service.py
--rw-rw-rw-   0        0        0      274 2024-04-10 01:35:46.315302 pih-bonus-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 01:35:46.284054 pih-bonus-0.1/pih_bonus.egg-info/
--rw-rw-rw-   0        0        0      274 2024-04-10 01:35:45.000000 pih-bonus-0.1/pih_bonus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-10 01:35:45.000000 pih-bonus-0.1/pih_bonus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 01:35:45.000000 pih-bonus-0.1/pih_bonus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-10 01:35:45.000000 pih-bonus-0.1/pih_bonus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 01:35:45.000000 pih-bonus-0.1/pih_bonus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-10 01:35:45.000000 pih-bonus-0.1/pih_bonus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 01:35:46.362186 pih-bonus-0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 02:21:12.774429 pih-bonus-0.11/
+drwxrwxrwx   0        0        0        0 2024-04-19 02:21:12.341264 pih-bonus-0.11/BonusProgramService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-bonus-0.11/BonusProgramService/__init__.py
+-rw-rw-rw-   0        0        0      154 2024-04-09 22:47:56.000000 pih-bonus-0.11/BonusProgramService/__main__.py
+-rw-rw-rw-   0        0        0     4076 2024-04-19 02:01:32.000000 pih-bonus-0.11/BonusProgramService/api.py
+-rw-rw-rw-   0        0        0      400 2024-04-19 02:06:48.000000 pih-bonus-0.11/BonusProgramService/const.py
+-rw-rw-rw-   0        0        0     5811 2024-04-19 01:51:55.000000 pih-bonus-0.11/BonusProgramService/service.py
+-rw-rw-rw-   0        0        0      275 2024-04-19 02:21:12.743182 pih-bonus-0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 02:21:12.711930 pih-bonus-0.11/pih_bonus.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-04-19 02:21:11.000000 pih-bonus-0.11/pih_bonus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2024-04-19 02:21:12.000000 pih-bonus-0.11/pih_bonus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 02:21:11.000000 pih-bonus-0.11/pih_bonus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-19 02:21:11.000000 pih-bonus-0.11/pih_bonus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-19 02:21:11.000000 pih-bonus-0.11/pih_bonus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-19 02:21:11.000000 pih-bonus-0.11/pih_bonus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 02:21:12.790094 pih-bonus-0.11/setup.cfg
```

